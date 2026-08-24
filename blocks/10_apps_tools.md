<a id="apps"></a>

## ▓ Apps & Tools

### LTX2.3-Multifunctional

**LTX2.3-Multifunctional** is a desktop-optimized version of LTX that lowers GPU requirements and simplifies usage. It integrates all features including image-to-video, text-to-video, start/end frames, lip-sync, video enhancement, and image generation into a single application.

**Key Features:**
- **Lower GPU Requirements**: Only needs 24GB VRAM (vs 32GB for standard desktop version)
- **All-in-One Interface**: No complex ComfyUI workflows or error-prone nodes
- **Features**: T2V, I2V, start/end frames, lip-sync, video enhancement, image generation, LoRA support
- **Multi-Frame Insertion**: Two modes for generating long videos
- **Easy Setup**: No third-party software required, just install LTX desktop

**Downloads & Resources:**
- [HuggingFace](https://huggingface.co/dx8152/LTX2.3-Multifunctional) | [GitHub](https://github.com/hero8152/LTX2.3-Multifunctional) | [ComfyUI Node](https://github.com/supart/ComfyUI_TY_LTX_Desktop_Bridge) | [Tutorial](https://youtu.be/rM_wUogtrOU)

### O2noor LTX-2.5 Int4 Tile-Train (Beta)

**O2noor LTX-2.5 Int4 Tile-Train** is a ComfyUI node pack for **LoRA training on LTX-2.5 22B distilled** using tiled training across multiple GPUs with as little as **18 GB VRAM** per card. The base is fully self-contained quantized weights (bnb-NF4 DiT, Gemma-4-12b text encoder — run in 8-bit LLM.int8 spread over 2 GPUs during captioning only, freed for training; works on 12 GB cards).

**Downloads & Resources:**
- [Node pack (GitHub)](https://github.com/A4ax/comfyui-LTX-2.5-Tile-train-LoRa--On-multi-Gpus-low-VRAM-18-gb-Beta) | [Model weights (HF)](https://huggingface.co/o2noor/comfyui-LTX-2.5-Tile-train-LoRa-On-multi-Gpus-low-VRAM-18-gb-Beta) — includes `ltx-2.5-22b-distilled-bnb-nf4` (10.45 GB), `embeddings_processor_bf16` (6.34 GB), `gemma4-12b-with-proj-ltx-2.5-bf16` (26.26 GB), video + audio VAEs, plus int2 experimental variants


