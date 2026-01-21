

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

  
## Workflows
