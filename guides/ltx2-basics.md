

## Model

### Checkpoint
```
📦 ComfyUI/
└── 📂 models/
    ├── 📂 checkpoints/
    │   └── ltx-2-19b-dev.safetensors
    ├── 📂 latent_upscale_models/
    │   └── ltx-2-spatial-upscaler-x2-1.0.safetensors
    ├── 📂 loras/
    │   └── ltx-2-19b-distilled-lora-384.safetensors
    └── 📂 text_encoders/
        └── gemma_3_12B_it_fp8_scaled.safetensors
```

### Split files

Loading splitted files:

| GGUF | Safetensors |
| :--- | :--- |
| <img alt="gguf" src="https://github.com/user-attachments/assets/61a7c429-f366-4176-af3b-28631358fa96" /> | <img alt="image" src="https://github.com/user-attachments/assets/8d7e0165-301f-4a8b-b163-2e091b67f7f5" /> |



### Settings

Common settings balance quality, speed, and hardware limits (VRAM/RAM).

| Parameter                  | Recommended Values                                                                 | Notes                                                                                          |
|----------------------------|-------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------|
| **Framerate**              | 25 FPS (default)  <br>48–50 FPS (high motion)  <br>15 FPS (static scenes)          | Audio latents are fixed at 25 FPS. Use Temporal Upscaler for 48/50 FPS to eliminate smearing. |
| **Resolution**             | 1280×720 (fast)  <br>1920×1080 (production)  <br>3840×2160 (4K, high-end only)     | Must be multiples of 32.                                                                      |
| **Video Length / Frames**  | 4–5 sec (~121 frames @ 25 FPS)  <br>Up to 20 sec (~481–505 frames)                  | Total frames must follow **1 + 8k** rule (9, 17, 121, 241, 481, etc.).                         |

#### Model Configuration
| Model Type | Steps | CFG | Notes |
| :--- | :--- | :--- | :--- |
| **Distilled** | 8 | 1.0 | Fastest results. |
| **Full / Dev** | 20–40 | 3.0–4.0 | Better prompt adherence. |


#### Hardware Optimization
*   **`--reserve-vram 2`** (or 1-5): Recommended for 24GB cards (RTX 3090/4090) to leave overhead for VAE decoding.
*   **`--cache-none`**: Forces VRAM offloading between steps. Recommended for systems with lower RAM/VRAM to prevent freezes.


## Quality & Performance Guide

To achieve production-grade results while maintaining reasonable generation times, the **2-Stage Generation Pipeline** is recommended.

### The 2-Stage Pipeline
The 2-stage approach involves generating a base video at a lower resolution and then upscaling it. This method is superior to native 1-stage generation for two key reasons:

1.  **Superior Motion Quality:** Native high-res generation often results in static motion or "mushy" details. The 2-stage pipeline utilizes a **Temporal Upscaler** to double the frame rate (e.g., 24fps $\to$ 48fps), significantly reducing "texture smearing" and "jiggle" in high-motion scenes.
2.  **Drastic Speed Improvements:** Generating 1080p in a single stage is extremely VRAM intensive. On consumer hardware (RTX 3090/4090), this often triggers offloading to system RAM, causing the system to freeze or generations to take upwards of **8 minutes**.
    *   *Comparison:* A 2-stage pass (Base Gen + Upscale) typically completes in **under 3 minutes**.

### Optimized Configuration
For the best balance of fidelity and speed, apply the following settings:

#### **Stage 1: Base Generation**
*   **Resolution:** 540p or 720p
*   **Model:** Full **Dev model**
*   **Steps:** 20–40 steps
*   **Goal:** Establish solid composition and fluid motion vectors.

#### **Stage 2: Upscaling & Refinement**
*   **Components:** Use **Spatial and Temporal Latent Upscalers** combined with the **Distilled LoRA**.
*   **Steps:** 3–8 steps (Fast refinement)
*   **CFG:** 1.0
*   **Goal:** Add fine texture details and sharpen the image without recalculating the scene geometry.

### The "48 FPS" Fix
To eliminate latent compression artifacts, **set your Stage 2 frame rate to 48 or 50 FPS.**
*   *Why?* Doubling the frame rate during the upscaling phase is the most effective method to counteract lossy compression, resulting in crisp, clear visuals.

  
## Workflows
