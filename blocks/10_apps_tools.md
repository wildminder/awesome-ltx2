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

### elismasilva LTX 2 Image Custom Blocks (Modular Diffusers)

Custom [Modular Diffusers](https://huggingface.co/docs/diffusers/main/en/modular_diffusers/overview) blocks that extend **LTX 2 Image** (elismasilva's image-only LTX-2.3) with **image-to-image**, plus a unified **`AutoBlocks`** pipeline that folds t2i and i2i into one — the workflow is chosen automatically from the inputs you pass (`prompt` → text-to-image; `prompt + image` → image-to-image with optional `strength`). Code-only repo (`trust_remote_code`); loads components from the [`ltx2.3-image-base`](https://huggingface.co/elismasilva/ltx2.3-image-base) weights repo. Apache-2.0.

**Downloads & Resources:**
- [Custom blocks (HF)](https://huggingface.co/elismasilva/ltx2.3_image_custom_blocks) | Image-only checkpoints: [ltx2.3-image-comfyui](https://huggingface.co/elismasilva/ltx2.3-image-comfyui) (ComfyUI) · [ltx2.3-image-base](https://huggingface.co/elismasilva/ltx2.3-image-base) (diffusers)

### WanGP LTX-2 Model Pack (DeepBeepMeep)

The complete set of **LTX-2 / 2.3 / 2.5 weights used by [WanGP](https://github.com/deepbeepmeep/Wan2GP)** — DeepBeepMeep's low-VRAM video app (down to ~6 GB VRAM, old-GPU friendly, auto-downloads the model variant matching your architecture). **169 files, ~984 GB total**, pre-packaged so no manual ComfyUI file layout is needed.

**What's inside:**
- **Main transformers (repo root)** — LTX-2.5 22B `dev` / `distilled` in bf16 (38.0 GB), int8-convrot (19.5 GB) and nvfp4 (14.7 GB); LTX-2.3 22B `dev` / `distilled` / `distilled-1.1` bf16 (38.0 GB) plus quanto bf16-int8 (19.5 GB) and nvfp4 (13.5 GB); LTX-2 19B `dev` / `distilled` full (43.3 GB), fp8 (27.1 GB), fp4 (20.0 GB) and diffusion-model variants; `Q4_K_M` / `Q6_K` / `Q8_0` "light" GGUFs (13.0–20.6 GB)
- **Third-party audio models** — JoyAI-Echo (bf16 + quanto), Scenema, DramaBox, `ltx23_echoVid-ltxAud_surgical_fp8`, plus Kokoro TTS, Seed-VC, Whisper, HuBERT, BigVGAN, Sherpa
- **Shared / offloadable components** — video + audio embeddings connectors (bf16 / int8-convrot / nvfp4), text embedding projection, video + audio VAEs, vocoder, spatial **and** temporal upscalers x2
- **Text encoders** — **both** `gemma4-12b-ltx-v1` for LTX-2.5 (bf16 23.8 GB / int8-convrot 12.9 GB) and `gemma-3-12b-it-qat-q4_0` for LTX-2 / 2.3 (24.4 GB + quanto 13.2 GB)
- **LoRAs** — LTX-2.5 IC-LoRAs (refine-details, ingredients, **SDR-To-HDR** + its `scene-emb`, deblur, decompression, pixel-spatial-upscaler), LTX-2.3 IC-LoRAs (ingredients, in-outpainting, outpaint, refocus, uncompress, ungrade, HDR + `scene-emb`, union-control, pixel-spatial-upscaler, detailer), LTX-2 IC-LoRAs (detailer, union-control, canny/depth/pose control), `distilled-lora-450` / `-384`, celebvhq **ID-LoRAs** (LTX-2 and 2.3), Edit-Anything reference, Licon-MSR (2.3 V1/V2, 2.5 V1 + slot embeddings), VBVR-I2V, OmniNFT RL-LoRAs
- **Manifest** — [`LTX-2.5-MANIFEST.md`](https://huggingface.co/DeepBeepMeep/LTX-2/blob/main/LTX-2.5-MANIFEST.md) documents the LTX-2.5 runtime set, incl. the note that Dev/Distilled connectors are shared only after equality verification and the official NVFP4 transformer needs its own BF16 connector pair

**Downloads & Resources:**
- [WanGP (GitHub)](https://github.com/deepbeepmeep/Wan2GP) | [Model pack (HF)](https://huggingface.co/DeepBeepMeep/LTX-2)

### LTX-2 Marking (VideoSeal / PixelSeal / AudioSeal)

The **weights and configs** for the opt-in, post-hoc invisible marking used by [LTX-2](https://github.com/Lightricks/LTX-2): **PixelSeal** (VideoSeal family) for video frames and **AudioSeal** for stereo PCM. MIT licensed, `pytorch` library. This is **not** a generator model - there is nothing to run or train against it, only to download.

| File | Purpose | Size | Download |
| :--- | :--- | :---: | :---: |
| `pixelseal.pth` | PixelSeal embedder + extractor weights (256-bit payload, 256 px processing size) | 308.95 MB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2-Marking/resolve/main/pixelseal.pth) |
| `audioseal_generator.pth` | AudioSeal 16-bit generator (embed) | 58.81 MB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2-Marking/resolve/main/audioseal_generator.pth) |
| `audioseal_detector.pth` | AudioSeal 16-bit detector | 34.67 MB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2-Marking/resolve/main/audioseal_detector.pth) |

**How it fits together** - the LTX-2 loader (`create_markers`) requires **all five model files** (the three above plus `pixelseal.yaml`, the PixelSeal model card describing the architecture, and `videoseal_attenuation.yaml`, the JND attenuation channel map) in one directory; the code that embeds and detects lives in `packages/ltx-pipelines/src/ltx_pipelines/marking` in the [LTX-2 repo](https://github.com/Lightricks/LTX-2). The `.pth` files are PyTorch pickles - verify the SHA-256 sums printed on the model card after download.

**Enable it** with `--marker-root-path path/to/marking` on the generation, editing and text-to-audio CLIs; omit the flag to leave pixels and PCM unchanged. Video generation and the HDR paths mark video while the text-to-audio path marks only audio, and detection returns `MarkDetectResult(detected, bit_accuracy, p_value, payload)` - video marks are judged on every 8th decoded frame at `log10(p_value) < -6`, audio over the full stereo track.

◦ The marks are a **robust invisible signal**, not a cryptographic signature: a detected mark means the clip came from an LTX-2 pipeline with marking enabled, while the absence of a mark does **not** prove a clip was not generated.

