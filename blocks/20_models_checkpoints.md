<a id="models"></a>

## ▓ Models

LTX-2 models are available in various formats including full weights, transformers-only, and GGUF quantizations for efficient inference.

<a id="checkpoints"></a>

<a id="ckpt"></a>

### ▣ Checkpoints

* **[Lightricks/LTX-2](https://huggingface.co/Lightricks/LTX-2)** - Official repository.
* **[Lightricks/LTX-2.3](https://huggingface.co/Lightricks/LTX-2.3)** - Official repository (latest version).
* **[Drbaph](https://huggingface.co/drbaph/LTX-2.3-FP8)** - Quantization
* **[unsloth](https://huggingface.co/unsloth)** - Quantized dev / distilled DiTs (FP8, INT8, INT8-ConvRot) + GGUF quants

| Ver | Name | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.5** | `dev` | ![bf16][badge-bf16] | 42.02 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5/resolve/main/diffusion_models/ltx-2.5-22b-dev-transformer-bf16.safetensors) |
| **2.5** | `dev` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 21.50 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5/resolve/main/diffusion_models/ltx-2.5-22b-dev-transformer-comfy-int8-convrot.safetensors) |
| **2.5** | `distilled` | ![bf16][badge-bf16] | 42.02 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5/resolve/main/diffusion_models/ltx-2.5-22b-distilled-transformer-bf16.safetensors) |
| **2.5** | `distilled` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 21.50 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5/resolve/main/diffusion_models/ltx-2.5-22b-distilled-transformer-comfy-int8-convrot.safetensors) |
| **2.5** | `distilled` | ![nvfp4][badge-nvfp4] | 18.72 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5/resolve/main/diffusion_models/ltx-2.5-22b-distilled-transformer-nvfp4.safetensors) |
| **2.5** | `pt` (pre-trained) | ![bf16][badge-bf16] | 46.2 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5-Pre-Trained/resolve/main/ltx-2.5-22b-pt-bf16.safetensors) |
| **2.5** | `distilled` | ![nvfp4][badge-nvfp4] | 22.1 GB | [![][gh-rockerBOO]](https://huggingface.co/rockerBOO/ltx-2.5-nvfp4-convrot/resolve/main/ltx-2.5-22b-distilled-transformer_nvfp4_convrot_int8.safetensors) |
| **2.5** | `dev` | ![w4a8_convrot](https://img.shields.io/badge/w4a8_ConvRot-17a2b8?style=flat-square) | 12.52 GB | [![][gh-Winnougan]](https://huggingface.co/Winnougan/ltx-2.5-w4a8-convrot-int4-convrot-Winnougan-Blessing/resolve/main/diffusion_models/ltx-2.5-22b-dev-transformer-w4a8_convrot.safetensors) |
| **2.5** | `distilled` | ![w4a8_convrot](https://img.shields.io/badge/w4a8_ConvRot-17a2b8?style=flat-square) | 12.52 GB | [![][gh-Winnougan]](https://huggingface.co/Winnougan/ltx-2.5-w4a8-convrot-int4-convrot-Winnougan-Blessing/resolve/main/diffusion_models/ltx-2.5-22b-distilled-transformer-w4a8_convrot.safetensors) |
| **2.5** | `distilled` | ![fp8][badge-fp8] | 21.03 GB | [![][gh-vonkaiser]](https://huggingface.co/vonkaiser/LTX-2.5-FP8-NVFP4/resolve/main/transformer/ltx-2.5-22b-distilled-fp8.safetensors) |
| **2.5** | `distilled` | ![nvfp4][badge-nvfp4] | 18.7 GB | [![][gh-BennyDaBall]](https://huggingface.co/BennyDaBall/LTX-2.5-22b-distilled-nvfp4-comfy/resolve/main/ltx-2.5-22b-distilled-transformer-nvfp4-comfy.safetensors) |
| **2.5** | `dev` | ![w4a8](https://img.shields.io/badge/w4a8-17a2b8?style=flat-square) | 15.4 GB | [![][gh-tsolful]](https://huggingface.co/tsolful/LTX_2.5_INT4_W4A8_ConvRot/resolve/main/ltx-2.5-22b-dev-transformer_W4A8_Mixed.safetensors) |
| **2.5** | `distilled` | ![w4a8](https://img.shields.io/badge/w4a8-17a2b8?style=flat-square) | 15.4 GB | [![][gh-tsolful]](https://huggingface.co/tsolful/LTX_2.5_INT4_W4A8_ConvRot/resolve/main/ltx-2.5-22b-distilled-transformer_W4A8_Mixed.safetensors) |
| **2.5** | `distilled` | ![fp8][badge-fp8] | 23.5 GB | [![][gh-guillaume127]](https://huggingface.co/guillaume127/LTX-2.5-FP8/resolve/main/ltx-2.5-22b-distilled-transformer-fp8_e4m3fn.safetensors) |
| **2.5** | `dev` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 21.64 GB | [![][gh-DmitryDB]](https://huggingface.co/DmitryDB/LTX-2.5-ComfyUI-Quants/resolve/main/diffusion_models/ltx-2.5-22b-dev-transformer-int8-convrot.safetensors) |
| **2.5** | `dev` | ![nvfp4][badge-nvfp4] | 13.57 GB | [![][gh-DmitryDB]](https://huggingface.co/DmitryDB/LTX-2.5-ComfyUI-Quants/resolve/main/diffusion_models/ltx-2.5-22b-dev-transformer-nvfp4.safetensors) |
| **2.5** | `distilled` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 21.64 GB | [![][gh-DmitryDB]](https://huggingface.co/DmitryDB/LTX-2.5-ComfyUI-Quants/resolve/main/diffusion_models/ltx-2.5-22b-distilled-transformer-int8-convrot.safetensors) |
| **2.5** | `distilled` | ![nvfp4][badge-nvfp4] | 13.57 GB | [![][gh-DmitryDB]](https://huggingface.co/DmitryDB/LTX-2.5-ComfyUI-Quants/resolve/main/diffusion_models/ltx-2.5-22b-distilled-transformer-nvfp4.safetensors) |
| **2.5** | `distilled` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 25.11 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2.5-FP8/resolve/main/LTX-2.5-INT8-ConvRot.safetensors) |
| **2.5** | `distilled` | ![fp8][badge-fp8] | 19.06 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2.5-FP8/resolve/main/LTX-2.5-FP8.safetensors) |
| **2.5** | `distilled` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 25.11 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2.5-FP8/resolve/main/LTX-2.5-INT8.safetensors) |
| | | | | |
| **2.3** | `dev` | ![bf16][badge-bf16] | 46.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-22b-dev.safetensors) |
| **2.3** | `dev` | ![fp8][badge-fp8] | 29.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3-fp8/resolve/main/ltx-2.3-22b-dev-fp8.safetensors) |
| **2.3** | `dev` | ![fp8][badge-fp8] | 29.9 GB | [![][gh-drbaph]](https://huggingface.co/drbaph/LTX-2.3-FP8/resolve/main/ltx-2.3-22b-dev-fp8.safetensors) |
| **2.3** | `dev` | ![int8mixedrowwise][badge-int8mixedrowwise] | 29.2 GB | [![][gh-Winnougan]](https://huggingface.co/Winnougan/LTX-2.3-Dev-Int8/resolve/main/ltx-2.3-22b-dev_int8mixed_rowwise.safetensors) |
| **2.3** | `dev` | ![nvfp4][badge-nvfp4] | 21.7 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3-nvfp4/resolve/main/ltx-2.3-22b-dev-nvfp4.safetensors) |
| **2.3** | `dev` | ![fp8][badge-fp8] | 29.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3-fp8/resolve/main/ltx-2.3-22b-dev-fp8.safetensors) |
| **2.3** | `distilled` | ![bf16][badge-bf16] | 46.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-22b-distilled.safetensors) |
| **2.3** | `distilled` | ![fp8][badge-fp8] | 29.5 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3-fp8/resolve/main/ltx-2.3-22b-distilled-fp8.safetensors) |
| **2.3** | `distilled` | ![fp8][badge-fp8] | 29.9 GB | [![][gh-drbaph]](https://huggingface.co/drbaph/LTX-2.3-FP8/resolve/main/ltx-2.3-22b-distilled-fp8.safetensors) |
| **2.3** | `distilled` | ![int8tensormixed][badge-int8tensormixed] | 29.1 GB | [![][gh-Winnougan]](https://huggingface.co/Winnougan/LTX-2.3-INT8/resolve/main/ltx-2.3-22b-distilled-int8tensormixed.safetensors) |
| **2.3** | `distilled` | ![nvfp4][badge-nvfp4] | 17.6 GB | [![][gh-Winnougan]](https://huggingface.co/Winnougan/LTX-2.3-INT8/resolve/main/ltx-2.3-22b-distilled_transformer_only_NVFP4.safetensors) |
| **2.3** | `distilled` | ![mxfp8mixed][badge-mxfp8mixed] | 29.7 GB | [![][gh-silveroxides]](https://huggingface.co/silveroxides/LTX-2.3-Quants/resolve/main/ltx-2.3-22b-distilled-mxfp8mixed.safetensors) |
| **2.3** | `distilled 1.1` | ![bf16][badge-bf16] | 46.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-22b-distilled-1.1.safetensors) |
| **2.3** | `distilled 1.1` | ![w4a8_convrot](https://img.shields.io/badge/w4a8_ConvRot-17a2b8?style=flat-square) | 16.65 GB | [![][gh-JoaoZaokk]](https://huggingface.co/JoaoZaokk/LTX-2.3-22B-distilled-1.1-W4A8-ConvRot/resolve/main/ltx-2.3-22b-distilled-1.1_w4a8.safetensors) |
| **2.3** | `distilled 1.1` | ![w4a4_convrot](https://img.shields.io/badge/w4a4_ConvRot-17a2b8?style=flat-square) | 15.37 GB | [![][gh-JoaoZaokk]](https://huggingface.co/JoaoZaokk/LTX-2.3-22B-distilled-1.1-W4A8-ConvRot/resolve/main/w4a4/ltx-2.3-22b-distilled-1.1_w4a4.safetensors) |
| **2.3** | `ltx23_srx fp8_e4m3 experimental` | ![fp8][badge-fp8] | 23.1 GB | [![][gh-SOLRICKS]](https://huggingface.co/SOLRICKS/ltx23_srx_fp8_e4m3_experimental/resolve/main/ltx23_srx_fp8_e4m3_experimental.safetensors) |
| **2.3** | `distilled` | ![fp8][badge-fp8] | 19.06 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2.3-FP8/resolve/main/LTX-2.3-FP8.safetensors) |
| **2.3** | `distilled` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 19.32 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2.3-FP8/resolve/main/LTX-2.3-INT8.safetensors) |
| | | | | |
| **2** | `ltx-2-19b dev` | ![bf16][badge-bf16] | 43.3 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-dev.safetensors) |
| **2** | `ltx-2-19b dev` | ![fp8][badge-fp8] | 27.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-dev-fp8.safetensors) |
| **2** | `ltx-2-19b dev` | ![fp4][badge-fp4] | 20 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-dev-fp4.safetensors) |
| **2** | `ltx-2-19b distilled` | ![bf16][badge-bf16] | 43.3 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-distilled.safetensors) |
| **2** | `ltx-2-19b distilled` | ![fp8][badge-fp8] | 27.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-distilled-fp8.safetensors) |
| **2** | `ltx-2-19b distilled` | ![nvfp4][badge-nvfp4] | 20 GB | [![](https://img.shields.io/badge/szwagros-lightgrey?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co/szwagros/ltx-2-dist-nvfp4/resolve/main/ltx-2-19b-distilled-nvfp4-fixed-calibrated.safetensors) |
| **2** | `ltx-2-19b dev` | ![fp8][badge-fp8] | 18.91 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-FP8/resolve/main/LTX-2-FP8.safetensors) |
| **2** | `ltx-2-19b dev` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 19.09 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-FP8/resolve/main/LTX-2-INT8.safetensors) |

◦ **unsloth quant rows** — pre-quantized DiTs built from the diffusers-format releases (torchao layout; loaded strictly by diffusers / Unsloth Studio — *not* ComfyUI single-file `diffusion_models/` weights). Each file is bit-identical to quantizing the dense bf16 weights on the fly, so it skips the dense load + quantize step. Repos: [LTX-2-FP8](https://huggingface.co/unsloth/LTX-2-FP8) (dev + pre-cast fp8 text encoder) · [LTX-2.3-FP8](https://huggingface.co/unsloth/LTX-2.3-FP8) (distilled + bf16 originals) · [LTX-2.5-FP8](https://huggingface.co/unsloth/LTX-2.5-FP8) (distilled; **INT8-ConvRot recommended**).

Quantized to fp8_e5m2 to support older Triton with older Pytorch on 30 series GPUs. For WangGP in Pinokio

| Ver | Name | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2** | `ltx-2-19b dev` | ![fp8_e5m2](https://img.shields.io/badge/fp8__e5m2-fe7d37?style=flat-square) | 27.1 GB | [![](https://img.shields.io/badge/progmars-lightgrey?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co/progmars/ltx-2-19b-dev-fp8_e5m2) |


<p id="ckpt-image-ltx23" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ Image-only LTX-2.3 (text-to-image)

Image-only **LTX-2.3** checkpoints by [elismasilva](https://huggingface.co/elismasilva) — the 13B LTX-2.3 family pruned to the still-image generation path (video/audio weights removed), packaged as unified ComfyUI safetensors. Inherits the LTX Video 2 Open Source License.

| Ver | Name | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.3** | `image dev` | ![bf16][badge-bf16] | 33.61 GB | [![elismasilva][gh-elismasilva]](https://huggingface.co/elismasilva/ltx2.3-image-comfyui/resolve/main/ltx-2.3-13b-image-dev.safetensors) |
| **2.3** | `image distilled` | ![bf16][badge-bf16] | 33.61 GB | [![elismasilva][gh-elismasilva]](https://huggingface.co/elismasilva/ltx2.3-image-comfyui/resolve/main/ltx-2.3-13b-image-distilled.safetensors) |
| **2.3** | `image dev` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 21.81 GB | [![elismasilva][gh-elismasilva]](https://huggingface.co/elismasilva/ltx2.3-image-comfyui/resolve/main/ltx-2.3-13b-image-dev-convrot-int8.safetensors) |
| **2.3** | `image distilled` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 21.81 GB | [![elismasilva][gh-elismasilva]](https://huggingface.co/elismasilva/ltx2.3-image-comfyui/resolve/main/ltx-2.3-13b-image-distilled-convrot-int8.safetensors) |

<p id="ckpt-silveroxides" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ silveroxides Quantizations (mxfp8)
**Note:** The mxfp8mixed quantization requires a [custom fork](https://huggingface.co/silveroxides/LTX-2.3-Quants) of ComfyUI-Kitchen with mxfp8 support. Standard ComfyUI installations may not support this quantization format.

| Model | Quant | Size | Download |
| :--- | :--- | :---: | :--- |
| `ltx-2.3-22b-dev` | ![int8mixedtensorwise][badge-int8mixedtensorwise] | 29.2 GB | [![][gh-silveroxides]](https://huggingface.co/silveroxides/LTX-2.3-Quants/resolve/main/ltx-2.3-22b-dev_int8mixedtensorwise.safetensors) |
| `ltx-2.3-22b-distilled` | ![int8tensormixed][badge-int8tensormixed] | 29.1 GB | [![][gh-silveroxides]](https://huggingface.co/silveroxides/LTX-2.3-Quants/resolve/main/ltx-2.3-22b-distilled-int8tensormixed.safetensors) |
| `ltx-2.3-22b-distilled` | ![int8mixedtensorwise][badge-int8mixedtensorwise] | 29.2 GB | [![][gh-silveroxides]](https://huggingface.co/silveroxides/LTX-2.3-Quants/resolve/main/ltx-2.3-22b-distilled-1.1_int8mixedtensorwise.safetensors) |
| `ltx-2.3-22b-distilled` | ![mxfp8mixed][badge-mxfp8mixed] | 29.7 GB | [![][gh-silveroxides]](https://huggingface.co/silveroxides/LTX-2.3-Quants/resolve/main/ltx-2.3-22b-distilled-mxfp8mixed.safetensors) |


<p id="ckpt-distilled-lora" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ Distilled LoRA

| Ver | Rank | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.5** | `450` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 5.06 GB | [![][gh-DmitryDB]](https://huggingface.co/DmitryDB/LTX-2.5-ComfyUI-Quants/resolve/main/loras/ltx-2.5-22b-distilled-lora-450-int8.safetensors) |
| **2.5** | `450` | ![nvfp4][badge-nvfp4] | 2.66 GB | [![][gh-DmitryDB]](https://huggingface.co/DmitryDB/LTX-2.5-ComfyUI-Quants/resolve/main/loras/ltx-2.5-22b-distilled-lora-450-nvfp4.safetensors) |
| **2.5** | `450` | ![bf16][badge-bf16] | 8.90 GB | [![][gh-rzgar]](https://huggingface.co/rzgar/ltx-2.5-22b-distilled-lora-450-enhanced-n4w/resolve/main/ltx-2.5-22b-distilled-lora-450-rank_450_n4w.safetensors) |
| **2.5** | `384` | ![bf16][badge-bf16] | 7.61 GB | [![][gh-rzgar]](https://huggingface.co/rzgar/ltx-2.5-22b-distilled-lora-450-enhanced-n4w/resolve/main/ltx-2.5-22b-distilled-lora-450-rank_384_n4w.safetensors) |
| **2.5** | `256` | ![bf16][badge-bf16] | 5.10 GB | [![][gh-rzgar]](https://huggingface.co/rzgar/ltx-2.5-22b-distilled-lora-450-enhanced-n4w/resolve/main/ltx-2.5-22b-distilled-lora-450-rank_256_n4w.safetensors) |
| **2.5** | `256` | ![bf16][badge-bf16] | 5.10 GB | [![][gh-TheDivergentAI]](https://huggingface.co/TheDivergentAI/ltx25-distill-lora/resolve/main/ltx25_turbo_distill_8step_r256.safetensors) |
| **2.5** | `128` | ![bf16][badge-bf16] | 2.58 GB | [![][gh-TheDivergentAI]](https://huggingface.co/TheDivergentAI/ltx25-distill-lora/resolve/main/ltx25_turbo_distill_8step_r128.safetensors) |
| **2.5** | `64` | ![bf16][badge-bf16] | 1.32 GB | [![][gh-TheDivergentAI]](https://huggingface.co/TheDivergentAI/ltx25-distill-lora/resolve/main/ltx25_turbo_distill_8step_r64.safetensors) |
| **2.5** | `128` | ![bf16][badge-bf16] | 2.31 GB | [![][gh-pyros-vault]](https://huggingface.co/pyros-vault/ltx-2.5-distilled-lora-450-reduced/resolve/main/ltx-2.5-22b-distilled-lora-450-bf16_fro90_ceil128.safetensors) |
| **2.5** | `72` | ![bf16][badge-bf16] | 1.38 GB | [![][gh-pyros-vault]](https://huggingface.co/pyros-vault/ltx-2.5-distilled-lora-450-reduced/resolve/main/ltx-2.5-22b-distilled-lora-450-bf16_fro90_ceil72.safetensors) |
| | | | | |
| **2.3** | `384` | ![bf16][badge-bf16] | 7.61 GB | [![](https://img.shields.io/badge/Lightricks_v1-lightgrey?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-22b-distilled-lora-384.safetensors) ┊ [![](https://img.shields.io/badge/Lightricks_v1.1-lightgrey?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-22b-distilled-lora-384-1.1.safetensors) |
| **2.3** | `208` | ![bf16][badge-bf16] | 4.97 GB | [![][gh-drbaph]](https://huggingface.co/drbaph/LTX-2.3-FP8/resolve/main/LoRA/ltx-2.3-22b-distilled-lora-resized_dynamic_rank_208_fro095_bf16.safetensors) |
| **2.3** | `159` | ![bf16][badge-bf16] | 3.83 GB | [![][gh-drbaph]](https://huggingface.co/drbaph/LTX-2.3-FP8/resolve/main/LoRA/ltx-2.3-22b-distilled-lora-resized_dynamic_rank_159_fro09_bf16.safetensors) |
| **2.3** | `111` | ![bf16][badge-bf16] | 2.74 GB | [![](https://img.shields.io/badge/Kijai_v1.1-lightgrey?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/loras/ltx-2.3-22b-distilled-1.1_lora-dynamic_fro09_avg_rank_111_bf16.safetensors) ┊ [![](https://img.shields.io/badge/Comfy--Org_v1.1-lightgrey?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co/Comfy-Org/ltx-2.3/resolve/main/split_files/loras/ltx_2.3_22b_distilled_1.1_lora_dynamic_fro09_avg_rank_111_bf16.safetensors) |
| **2.3** | `105` | ![bf16][badge-bf16] | 2.59 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/loras/ltx-2.3-22b-distilled-lora-dynamic_fro09_avg_rank_105_bf16.safetensors) |
| | | | | |
| **2** | `384` | ![bf16][badge-bf16] | 7.67 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-distilled-lora-384.safetensors) |
| **2** | `242` | ![bf16][badge-bf16] | 4.88 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/loras/ltx-2-19b-distilled-lora-resized_dynamic_fro095_avg_rank_242_bf16.safetensors) |
| **2** | `175` | ![bf16][badge-bf16] | 3.58 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/loras/ltx-2-19b-distilled-lora_resized_dynamic_fro09_avg_rank_175_bf16.safetensors) |
| **2** | `175` | ![fp8][badge-fp8] | 1.79 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/loras/ltx-2-19b-distilled-lora_resized_dynamic_fro09_avg_rank_175_fp8.safetensors) |


<p id="ckpt-tenstrip-distilled-lora" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ TenStrip Distilled LoRA Experiments
Experimental distilled LoRAs optimized for finetunes and I2V workflows. These LoRAs avoid the issues of the massive rank 384 official LoRA which can be counterproductive with conditioned inputs and finetunes.

| Name | Rank | Mode | Size | Download |
|:---|:---:|:---|:---:|:---:|
| `distilled v1.1` | `32` | condsafe | 380 MB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments/resolve/main/ltx-2.3-22b-distilled-lora-1.1_fro90_ceil32_condsafe.safetensors) |
| `distilled v1.1` | `36` | — | 739 MB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments/resolve/main/ltx-2.3-22b-distilled-lora-1.1_fro90_ceil36.safetensors) |
| `distilled v1.1` | `52` | condsafe | 487 MB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments/resolve/main/ltx-2.3-22b-distilled-lora-1.1_fro90_ceil52_condsafe.safetensors) |
| `distilled v1.1` | `72` | condsafe | 662 MB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments/resolve/main/ltx-2.3-22b-distilled-lora-1.1_fro90_ceil72_condsafe.safetensors) |
| `distilled` | `72` | — | 1.4 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments/resolve/main/ltx-2.3-22b-distilled-lora-fro90_ceil72.safetensors) |
| `distilled v1.1` | `72` | energy | 1.72 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments/resolve/main/ltx-2.3-22b-distilled-lora-1.1_rank72_energy.safetensors) |
| `distilled v1.1` | `96` | energy | 2.28 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments/resolve/main/ltx-2.3-22b-distilled-lora-1.1_rank96_energy.safetensors) |

**Notes:**
- Lower rank LoRAs (72 and below) can be used at 1.0 strength safely for I2V first pass, with upscale pass at 0.4-0.5 strength
- `_ceil` suffix indicates the dynamic ceiling during reranking
- `_condsafe` suffix indicates cross-attention and other conditioning layers have been zeroed for better I2V compatibility
- The official rank 384 LoRA can actively dampen conditioning signals in I2V workflows; cond_safe versions work much better

[Download All LoRAs](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments)


<p id="ckpt-spatial-upscaler" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ Spatial Upscaler

Required for current two-stage pipeline implementations in this repository. Download to `COMFYUI_ROOT_FOLDER/models/latent_upscale_models` folder.

| Ver | Name | Size | Download |
| :--- | :--- | :--- | :--- |
| **2.5** | `spatial-upscaler x2 1.0` | 995.78 MB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5/resolve/main/latent_upscale_models/ltx-2.5-latent-spatial-upscaler-x2-bf16-1.0.safetensors) ┊ [![][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.5-uncensored-v1.1-FP8/resolve/main/split/latent_upscale_models/ltx-2.5-latent-spatial-upscaler-x2-bf16-1.0.safetensors) |
| **2.3** | `spatial-upscaler x2 1.0` | 996 MB | [![][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.3-uncensored-v1.4-FP8/resolve/main/split/latent_upscale_models/ltx-2.3-spatial-upscaler-x2-1.0.safetensors) |
| **2.3** | `spatial-upscaler x2 1.1` | 996 MB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-spatial-upscaler-x2-1.1.safetensors) ┊ [![][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.3-uncensored-v1.4-FP8/resolve/main/split/latent_upscale_models/ltx-2.3-spatial-upscaler-x2-1.1.safetensors) |
| **2.3** | `spatial-upscaler x1.5 1.0` | 1.09 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-spatial-upscaler-x1.5-1.0.safetensors) |
| | | | |
| **2** | `spatial-upscaler x2 1.0` | 995.77 MB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-spatial-upscaler-x2-1.0.safetensors) |

⚠️ The official `ltx-2.3-spatial-upscaler-x2-1.0.safetensors` was **deleted upstream** from `Lightricks/LTX-2.3`; only the **ChrisColeTech** mirror still carries the 1.0 build. The upstream successor is **x2 1.1** (linked above) — the repo now ships `x1.5 1.0` and `x2 1.1` only.


<p id="ckpt-temporal-upscaler" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ Temporal Upscaler

Required for current two-stage pipeline implementations in this repository. Download to `COMFYUI_ROOT_FOLDER/models/latent_upscale_models` folder.

| Ver | Name | Size | Download |
| :--- | :--- | :--- | :--- |
| **2.5** | `temporal-upscaler x2 1.0` | 0.26 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5/resolve/main/latent_upscale_models/ltx-2.5-latent-temporal-upscaler-x2-bf16-1.0.safetensors) ┊ [![][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.5-uncensored-v1.1-FP8/resolve/main/split/latent_upscale_models/ltx-2.5-latent-temporal-upscaler-x2-bf16-1.0.safetensors) |
| **2.3** | `temporal-upscaler x2 1.0` | 262 MB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-temporal-upscaler-x2-1.0.safetensors) |
| | | | |
| **2** | `temporal-upscaler x2 1.0` | 262 MB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-temporal-upscaler-x2-1.0.safetensors) |

<p id="merges" align="center">══════════════════════════════════</p>

### ▣ Merges

Custom merged models combining multiple control signals or specialized configurations.

| Ver | Name | Description | Download |
| :--- | :--- | :--- | :--- |
| **2.3** | `ltx-2.3-22b-distilled-1.1-fused-union-control` | Merged model combining Canny, Depth, and Pose control signals for unified control | [![](https://img.shields.io/badge/linoyts-lightgrey?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co/linoyts/ltx-2.3-22b-distilled-1.1-fused-union-control) |
| **2.5** | `Alpha-Gen VideoOnly48 NVFP4` | Official Alpha-Gen IC-LoRA **merged into the base weights** at strength 1.0, then structurally pruned to 48 blocks and quantized to NVFP4 with dynamic activation scales. Ships no LoRA — the matting behaviour is in the checkpoint. Ships a `provenance.json` with base/alpha SHA-256 and a full quality-vs-teacher report. | [![](https://img.shields.io/badge/mskim8584-lightgrey?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co/mskim8584/LTX-2.5-Alpha-Gen-VideoOnly-NVFP4/resolve/main/ltx25-alpha-gen-videoonly48-merged-nvfp4-dynamic.safetensors) |

◦ **mskim8584 caveats — read `provenance.json` before trusting it.** The producer's own audit reports `"quality_accepted": false` and `"accepted": false`: whole-frame MAE 0.0059, PSNR 30.8 dB, SSIM 0.972, gradient MAE 0.0042, temporal flicker MAE 0.0034, temporal-boundary MAE 0.0416. `catastrophic_inversion_frame_count` is 0, so nothing blew up, but both the BF16 intermediate and the NVFP4 pass were explicitly marked as *not* accepted quality. The BF16 merge also required `cached_final_empty_prompt_required` conditioning and was fused on CPU. Treat as an experiment, not a drop-in replacement for the LoRA.

<p id="finetunes" align="center">══════════════════════════════════</p>

### ▣ Finetunes

Community finetuned models based on LTX-2.3 with specialized improvements and optimizations. Each finetune family may include a backbone checkpoint, low-VRAM component splits, GGUF quants, and merged or extracted LoRAs. Variant cell links go directly to the resolve/main safetensors/gguf file when a single canonical asset covers the row.

<a id="finetune-dasiwa"></a>

#### ❖ DaSiWa

High-performance LoRA-integrated checkpoint family based on LTX 2.3. Includes distilled (4-step) and non-distilled (20-30 step) variants. Recommended sampler: Euler + Simple/Normal/Linear_Quadratic.

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **2.3** | Distilled | `Treasurechest V1` | ![fp8][badge-fp8] | 21.02 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Distilled/FP8/v01/DasiwaLTX23Lightspeed_treasurechestV1.safetensors) |
| **2.3** | Distilled | `Solsticecoin V2` | ![fp8][badge-fp8] | 30.13 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Distilled/FP8/v03/DasiwaLTX23_solsticecoinV2-fp8.safetensors) |
| **2.3** | Distilled | `Dragonleap V4` | ![int4mixedtensorwise][badge-int4mixedtensorwise] | 18.38 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Distilled/DasiwaLTX23_dragonleapV4-INT4%20ConvRot.safetensors) |
| **2.3** | Distilled | `Dragonleap V4` | ![int8tensormixed][badge-int8tensormixed] | 27.64 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Distilled/DasiwaLTX23_dragonleapV4-INT8%20ConvRot.safetensors) |
| **2.3** | Non-Distilled | `GoldenLace V3` | ![fp8][badge-fp8] | 29.16 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/FP8/v03/DasiwaLTX23_goldenLaceV3-fp8.safetensors) |
| **2.3** | Non-Distilled | `GoldenLace V3` | ![nvfp4][badge-nvfp4] | 21.73 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/NVFP4/v03/DasiwaLTX23_goldenLaceV3-fp4.safetensors) |
| **2.3** | Non-Distilled GGUF | `GoldenLace V3` | ![Q2_K][badge-Q2_K] | 8.51 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/GGUF/v03/DasiwaLTX23_goldenLaceV3-Q2_K.gguf) |
| **2.3** | Non-Distilled GGUF | `GoldenLace V3` | ![Q3_K_M][badge-Q3_K_M] | 10.6 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/GGUF/v03/DasiwaLTX23_goldenLaceV3-Q3_K_M.gguf) |
| **2.3** | Non-Distilled GGUF | `GoldenLace V3` | ![Q4_K_M][badge-Q4_K_M] | 13.33 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/GGUF/v03/DasiwaLTX23_goldenLaceV3-Q4_K_M.gguf) |
| **2.3** | Non-Distilled GGUF | `GoldenLace V3` | ![Q5_K_M][badge-Q5_K_M] | 15.9 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/GGUF/v03/DasiwaLTX23_goldenLaceV3-Q5_K_M.gguf) |
| **2.3** | Non-Distilled GGUF | `GoldenLace V3` | ![Q6_K][badge-Q6_K] | 18.63 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/GGUF/v03/DasiwaLTX23_goldenLaceV3-Q6_K.gguf) |
| **2.3** | Non-Distilled GGUF | `GoldenLace V3` | ![Q8_0][badge-Q8_0] | 23.61 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/GGUF/v03/DasiwaLTX23_goldenLaceV3-Q8_0.gguf) |

**DaSiWa extracted LoRA:**

| Build | Name | LoRA Rank | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| DMD v2 audio | `LTX2.3_DMD_v2_avgrank86_audio160_L80-D20` | 86 (audio 160) | 2.27 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Lora/LTX2.3_DMD_v2_avgrank86_audio160_L80-D20.safetensors) |

<p id="finetune-10eros" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ 10Eros

I2V-optimised merge using layer scaled merges at different steps. Not a straight weight merge — behaves much nicer than standard LoRA loading and respects prompts.

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **2.3** | Full | `10Eros v1` | ![bf16][badge-bf16] | 46.14 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1_bf16.safetensors) |
| **2.3** | Full | `10Eros v1` | ![fp8][badge-fp8] | 29.16 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1-fp8mixed_learned.safetensors) |
| **2.3** | transformer-only | `10Eros v1` | ![fp8][badge-fp8] | 29.56 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1_fp8_transformer.safetensors) |
| **2.3** | Full | `10Eros v1.2` | ![bf16][badge-bf16] | 46.14 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1.2_bf16.safetensors) |
| **2.3** | Full | `10Eros v1.2` | ![fp8][badge-fp8] | 34.33 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1.2_fp8mixed_learned.safetensors) |
| **2.3** | Full | `10Eros v1.3` | ![bf16][badge-bf16] | 46.14 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1.3_bf16.safetensors) |
| **2.3** | Full | `10Eros v1.3` | ![fp8][badge-fp8] | 29.16 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1.3_fp8mixed_learned.safetensors) |
| **2.3** | Full | `10Eros v1.4` | ![bf16][badge-bf16] | 46.14 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1.4_bf16.safetensors) |
| **2.3** | Full | `10Eros v1.4` | ![fp8][badge-fp8] | 29.16 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1.4_fp8mixed_learned.safetensors) |
| **2.3** | Full | `10Eros v1.4 DMD int8 ConvRot` | ![int8tensormixed][badge-int8tensormixed] | 29.16 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/INT8%20diffusion_models/10Eros_v1.4_DMD_int8_convrot.safetensors) |
| **2.3** | Full | `10Eros v1.5` | ![bf16][badge-bf16] | 46.14 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1.5_bf16.safetensors) |
| **2.3** | Full | `10Eros v1.5 DMD int8` | ![int8tensormixed][badge-int8tensormixed] | 29.16 GB | [![CornLogic][gh-CornLogic]](https://huggingface.co/CornLogic/10EROS-INT8/resolve/main/10Eros_v1.5_DMD_INT8_checkpoint.safetensors) |
| **2.3** | transformer-only | `10Eros v1.5 DMD int8` | ![int8tensormixed][badge-int8tensormixed] | 25.03 GB | [![CornLogic][gh-CornLogic]](https://huggingface.co/CornLogic/10EROS-INT8/resolve/main/10Eros_v1.5_INT8_DMD_TFO.safetensors) |
| **2.3** | transformer-only | `10Eros v1.5 int8` | ![int8tensormixed][badge-int8tensormixed] | 25.03 GB | [![CornLogic][gh-CornLogic]](https://huggingface.co/CornLogic/10EROS-INT8/resolve/main/10Eros_v1.5_INT8_TFO.safetensors) |
| **2.3** | Full | `10Eros v1.5 fp8mixed (experimental, learned)` | ![fp8][badge-fp8] | 30.24 GB | [![LokkenJP][gh-LokkenJP]](https://huggingface.co/LokkenJP/10EROS_1.5_fp8_exp_learned/resolve/main/10Eros_v1.5_fp8mixed_experimental_learned.safetensors) |
| **2.3** | Full | `10Eros v1 INT8 ConvRot` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 23.51 GB | [![milo01][gh-milo01]](https://huggingface.co/milo01/LTX2.3-10Eros-INT8-ConvRot/resolve/main/10Eros_v1_bf16-int8.ConvRot.safetensors) |

◦ **The `10Eros Max` line is a different architecture — see [`❖ 10Eros Max (MiniMax-H3 grafts)`](#finetune-10eros-max-h3) below.** The gated `TenStrip/LTX2.3-10Eros_Version-Testing` repo despite its name holds **MiniMax-H3 (Hailuo 3)** grafts, **not** LTX-2.3 DiTs. Everything in the table above is a genuine LTX-2.3 `AVTransformer3DModel` checkpoint (`model.diffusion_model` + `vocoder` + `vae` + `audio_vae`, 23.07 B params).

◦ **`10Eros v1.5` companions** — the int8 and fp8mixed v1.5 builds live in third-party repos: [CornLogic/10EROS-INT8](https://huggingface.co/CornLogic/10EROS-INT8) (full int8 checkpoint + two transformer-only variants) and [LokkenJP/10EROS_1.5_fp8_exp_learned](https://huggingface.co/LokkenJP/10EROS_1.5_fp8_exp_learned) (fp8mixed, experimental, with a `.quantization.json` + `.sha256` sidecar).

◦ **`10Eros v1 INT8 ConvRot` mirror** — the original `bertbobson/LTX2.3-10Eros-INT8-ConvRot` repo is **no longer public** (the API returns `Invalid username or password` and it is absent from the author's model list). The row above points at the public [milo01/LTX2.3-10Eros-INT8-ConvRot](https://huggingface.co/milo01/LTX2.3-10Eros-INT8-ConvRot) mirror, which carries the identically-named file at the same byte size. Other public mirrors: [Winnougan/10Eros-INT8-Convrot](https://huggingface.co/Winnougan/10Eros-INT8-Convrot) (v1.2), [CornLogic/10EROS_1.4_Int8_ConvRot](https://huggingface.co/CornLogic/10EROS_1.4_Int8_ConvRot) and [chfm/10EROS_1.4_Int8_ConvRot](https://huggingface.co/chfm/10EROS_1.4_Int8_ConvRot) (v1.4, both).

◦ **10Eros GGUF** — vantagewithai low-VRAM quants

<details>
  <summary>vantagewithai/LTX2.3-10Eros-GGUF</summary>

[`vantagewithai/LTX2.3-10Eros-GGUF`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF) — v1

| Quant | Size | Download |
| :--- | :---: | :--- |
| ![Q3_K_M][badge-Q3_K_M] | 11.13 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q3_K_M.gguf) |
| ![Q3_K_S][badge-Q3_K_S] | 10.34 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q3_K_S.gguf) |
| ![Q4_0][badge-Q4_0] | 12.98 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q4_0.gguf) |
| ![Q4_1][badge-Q4_1] | 13.9 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q4_1.gguf) |
| ![Q4_K_M][badge-Q4_K_M] | 14.3 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q4_K_M.gguf) |
| ![Q4_K_S][badge-Q4_K_S] | 13.2 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q4_K_S.gguf) |
| ![Q5_0][badge-Q5_0] | 15.26 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q5_0.gguf) |
| ![Q5_1][badge-Q5_1] | 16.18 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q5_1.gguf) |
| ![Q5_K_M][badge-Q5_K_M] | 16.14 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q5_K_M.gguf) |
| ![Q5_K_S][badge-Q5_K_S] | 15.04 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q5_K_S.gguf) |
| ![Q6_K][badge-Q6_K] | 17.77 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q6_K.gguf) |
| ![Q8_0][badge-Q8_0] | 22.76 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q8_0.gguf) |

</details>

<details>
  <summary>vantagewithai/LTX2.3-10Eros-1.2-GGUF</summary>

[`vantagewithai/LTX2.3-10Eros-1.2-GGUF`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF) — v1.2 — **Note:** files are named `10Eros_v1.210Eros_v1.2-…gguf` (upstream double-stamp glitch); we link verbatim.

| Quant | Size | Download |
| :--- | :---: | :--- |
| ![Q3_K_M][badge-Q3_K_M] | 11.13 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q3_K_M.gguf) |
| ![Q3_K_S][badge-Q3_K_S] | 10.34 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q3_K_S.gguf) |
| ![Q4_0][badge-Q4_0] | 12.98 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q4_0.gguf) |
| ![Q4_1][badge-Q4_1] | 13.9 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q4_1.gguf) |
| ![Q4_K_M][badge-Q4_K_M] | 14.3 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q4_K_M.gguf) |
| ![Q4_K_S][badge-Q4_K_S] | 13.2 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q4_K_S.gguf) |
| ![Q5_0][badge-Q5_0] | 15.26 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q5_0.gguf) |
| ![Q5_1][badge-Q5_1] | 16.18 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q5_1.gguf) |
| ![Q5_K_M][badge-Q5_K_M] | 16.14 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q5_K_M.gguf) |
| ![Q5_K_S][badge-Q5_K_S] | 15.04 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q5_K_S.gguf) |
| ![Q6_K][badge-Q6_K] | 17.77 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q6_K.gguf) |
| ![Q8_0][badge-Q8_0] | 22.76 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q8_0.gguf) |

</details>

<details>
  <summary>vantagewithai/LTX2.3-10Eros-1.3-GGUF</summary>

[`vantagewithai/LTX2.3-10Eros-1.3-GGUF`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF) — v1.3

| Quant | Size | Download |
| :--- | :---: | :--- |
| ![Q3_K_M][badge-Q3_K_M] | 11.13 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q3_K_M.gguf) |
| ![Q3_K_S][badge-Q3_K_S] | 10.34 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q3_K_S.gguf) |
| ![Q4_0][badge-Q4_0] | 12.98 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q4_0.gguf) |
| ![Q4_1][badge-Q4_1] | 13.9 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q4_1.gguf) |
| ![Q4_K_M][badge-Q4_K_M] | 14.3 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q4_K_M.gguf) |
| ![Q4_K_S][badge-Q4_K_S] | 13.2 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q4_K_S.gguf) |
| ![Q5_0][badge-Q5_0] | 15.26 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q5_0.gguf) |
| ![Q5_1][badge-Q5_1] | 16.18 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q5_1.gguf) |
| ![Q5_K_M][badge-Q5_K_M] | 16.14 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q5_K_M.gguf) |
| ![Q5_K_S][badge-Q5_K_S] | 15.04 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q5_K_S.gguf) |
| ![Q6_K][badge-Q6_K] | 17.77 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q6_K.gguf) |
| ![Q8_0][badge-Q8_0] | 22.76 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q8_0.gguf) |

</details>

<details>
  <summary>vantagewithai/LTX2.3-10Eros-1.4-GGUF</summary>

[`vantagewithai/LTX2.3-10Eros-1.4-GGUF`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF) — v1.4 (latest)

| Quant | Size | Download |
| :--- | :---: | :--- |
| ![Q3_K_M][badge-Q3_K_M] | 11.13 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q3_K_M.gguf) |
| ![Q3_K_S][badge-Q3_K_S] | 10.34 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q3_K_S.gguf) |
| ![Q4_0][badge-Q4_0] | 12.98 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q4_0.gguf) |
| ![Q4_1][badge-Q4_1] | 13.9 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q4_1.gguf) |
| ![Q4_K_M][badge-Q4_K_M] | 14.3 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q4_K_M.gguf) |
| ![Q4_K_S][badge-Q4_K_S] | 13.2 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q4_K_S.gguf) |
| ![Q5_0][badge-Q5_0] | 15.26 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q5_0.gguf) |
| ![Q5_1][badge-Q5_1] | 16.18 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q5_1.gguf) |
| ![Q5_K_M][badge-Q5_K_M] | 16.14 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q5_K_M.gguf) |
| ![Q5_K_S][badge-Q5_K_S] | 15.04 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q5_K_S.gguf) |
| ![Q6_K][badge-Q6_K] | 17.77 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q6_K.gguf) |
| ![Q8_0][badge-Q8_0] | 22.76 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q8_0.gguf) |

</details>

<details>
  <summary>vantagewithai/LTX2.3-10Eros-1.5-GGUF</summary>

[`vantagewithai/LTX2.3-10Eros-1.5-GGUF`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.5-GGUF) — v1.5 (latest)

| Quant | Size | Download |
| :--- | :---: | :--- |
| ![Q3_K_M][badge-Q3_K_M] | 11.13 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.5-GGUF/resolve/main/10Eros_v1.5-Q3_K_M.gguf) |
| ![Q3_K_S][badge-Q3_K_S] | 10.34 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.5-GGUF/resolve/main/10Eros_v1.5-Q3_K_S.gguf) |
| ![Q4_0][badge-Q4_0] | 12.98 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.5-GGUF/resolve/main/10Eros_v1.5-Q4_0.gguf) |
| ![Q4_1][badge-Q4_1] | 13.90 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.5-GGUF/resolve/main/10Eros_v1.5-Q4_1.gguf) |
| ![Q4_K_M][badge-Q4_K_M] | 14.30 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.5-GGUF/resolve/main/10Eros_v1.5-Q4_K_M.gguf) |
| ![Q4_K_S][badge-Q4_K_S] | 13.20 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.5-GGUF/resolve/main/10Eros_v1.5-Q4_K_S.gguf) |
| ![Q5_0][badge-Q5_0] | 15.26 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.5-GGUF/resolve/main/10Eros_v1.5-Q5_0.gguf) |
| ![Q5_1][badge-Q5_1] | 16.18 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.5-GGUF/resolve/main/10Eros_v1.5-Q5_1.gguf) |
| ![Q5_K_M][badge-Q5_K_M] | 16.14 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.5-GGUF/resolve/main/10Eros_v1.5-Q5_K_M.gguf) |
| ![Q5_K_S][badge-Q5_K_S] | 15.04 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.5-GGUF/resolve/main/10Eros_v1.5-Q5_K_S.gguf) |
| ![Q6_K][badge-Q6_K] | 17.77 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.5-GGUF/resolve/main/10Eros_v1.5-Q6_K.gguf) |
| ![Q8_0][badge-Q8_0] | 22.76 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.5-GGUF/resolve/main/10Eros_v1.5-Q8_0.gguf) |

</details>

◦ **10Eros Splits**
<details>
  <summary>per-version component split</summary>

[`vantagewithai/LTX2.3-10Eros-Split`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-Split) — v1
| Component | Precision | Size | Download |
| :--- | :---: | :---: | :--- |
| Model | ![bf16][badge-bf16] | 42.01 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-Split/resolve/main/model/10Eros_v1_bf16_model.safetensors) |
| Model | ![fp8][badge-fp8] | 28.28 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-Split/resolve/main/model/10Eros_v1_fp8_model.safetensors) |
| VAE | — | 1.45 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-Split/resolve/main/vae/10Eros_v1_vae.safetensors) |
| Audio VAE | — | 364.86 MB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-Split/resolve/main/audio_vae/10Eros_v1_audio_vae.safetensors) |
| Text encoder | — | 2.31 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-Split/resolve/main/text_encoder/10Eros_v1_text_encoder.safetensors) |

[`vantagewithai/LTX2.3-10Eros-1.2-Split`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-Split) — v1.2
| Component | Precision | Size | Download |
| :--- | :---: | :---: | :--- |
| Model | ![bf16][badge-bf16] | 42.01 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-Split/resolve/main/model/10Eros_v1.2_bf16_model.safetensors) |
| Model | ![fp8][badge-fp8] | 30.2 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-Split/resolve/main/model/10Eros_v1.2_fp8mixed_learned_model.safetensors) |
| VAE | — | 1.45 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-Split/resolve/main/vae/10Eros_v1.2_vae.safetensors) |
| Audio VAE | — | 364.86 MB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-Split/resolve/main/audio_vae/10Eros_v1.2_audio_vae.safetensors) |
| LoRA (bundled) | — | 662.07 MB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-Split/resolve/main/lora/ltx-2.3-22b-distilled-lora-1.1_fro90_ceil72_condsafe.safetensors) |

[`vantagewithai/LTX2.3-10Eros-1.3-Split`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-Split) — v1.3
| Component | Precision | Size | Download |
| :--- | :---: | :---: | :--- |
| Model | ![bf16][badge-bf16] | 42.01 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-Split/resolve/main/model/10Eros_v1.3_bf16_model.safetensors) |
| Model | ![fp8][badge-fp8] | 25.03 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-Split/resolve/main/model/10Eros_v1.3_fp8mixed_learned_model.safetensors) |
| VAE | — | 1.45 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-Split/resolve/main/vae/10Eros_v1.3_vae.safetensors) |
| Audio VAE | — | 364.86 MB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-Split/resolve/main/audio_vae/10Eros_v1.3_audio_vae.safetensors) |
| Text encoder | — | 2.31 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-Split/resolve/main/text_encoder/10Eros_v1.3_text_encoder.safetensors) |

[`vantagewithai/LTX2.3-10Eros-1.4-Split`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-Split) — v1.4 (latest)
| Component | Precision | Size | Download |
| :--- | :---: | :---: | :--- |
| Model | ![bf16][badge-bf16] | 42.01 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-Split/resolve/main/model/10Eros_v1.4_bf16_model.safetensors) |
| Model | ![fp8][badge-fp8] | 25.03 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-Split/resolve/main/model/10Eros_v1.4_fp8mixed_learned_model.safetensors) |
| VAE | — | 1.45 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-Split/resolve/main/vae/10Eros_v1.4_vae.safetensors) |
| Audio VAE | — | 364.86 MB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-Split/resolve/main/audio_vae/10Eros_v1.4_audio_vae.safetensors) |
| Text encoder | — | 2.31 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-Split/resolve/main/text_encoder/10Eros_v1.4_text_encoder.safetensors) |


</details>

◦ **10Eros Splits** — AX1Y2JP transformer-only fork (alternative split for ComfyUI)

| Variant | Download |
| :--- | :--- |
| v1.4 transformer_only bf16 | [![AX1Y2JP][gh-AX1Y2JP]](https://huggingface.co/AX1Y2JP/LTX2.3-10Eros_split/resolve/main/diffusion_models/10Eros_v1.4_transformer_only_bf16.safetensors) |
| v1.4 transformer_only fp8mixed_learned | [![AX1Y2JP][gh-AX1Y2JP]](https://huggingface.co/AX1Y2JP/LTX2.3-10Eros_split/resolve/main/diffusion_models/10Eros_v1.4_transformer_only_fp8mixed_learned.safetensors) |
| v1.4 video VAE bf16 | [![AX1Y2JP][gh-AX1Y2JP]](https://huggingface.co/AX1Y2JP/LTX2.3-10Eros_split/resolve/main/vae/10Eros_v1.4_video_vae_bf16.safetensors) |

◦ **10Eros Extracted LoRA** — maximsobolev275 trained LoRAs

| Variant | Description | Download |
| :--- | :--- | :--- |
| rank-768 family (canonical, v1.4) | Author: maximsobolev275. Training LoRAs directly extracted from the 10Eros v1.4 merge (rank 768); lower-rank rerolls for v1.2 / v1.3 / v1.4 are also published in the same repo. | [LTX-10Eros-LoRA-r768](https://huggingface.co/maximsobolev275/LTX-10Eros-LoRA-r768) |

◦ **10Eros distilled-baked collection** — ibyteohdear

Massive 10Eros **distilled-baked** checkpoint collection by [ibyteohdear](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros) — 20 safetensors of full LTX distilled checkpoints with the 10Eros style baked in. The repo was **restructured on 2026-10-26**, so the catalogue below was rebuilt from the live tree: the earlier r64 / r128 / r768 / r768_0.85 builds and the bundled `JoyAI-Echo_r256` / reasoning I2V LoRAs are gone.

◦ **LTX-2.3** — `LTX2.3_DISTILLED_BAKED_LTX_SULPHUR_STYLE_IS_10Eros_v{1,12,13,14,15}_r{256,512}` — **full checkpoints** (DiT + `vocoder` + video/audio `vae` + `text_embedding_projection`; 5,947 tensors, all BF16, `model_version 2.3.0`, config `AVTransformer3DModel`), baked from the **Sulphur-2** base with the 10Eros style merged in.

◦ **LTX-2.5** — `LTX2.5_DISTILLED_STYLE_10Eros_{1,12,13,14,15}[_SULPHUR]_r512_audio_r256_rest_0` — **transformer-only** (`model.diffusion_model.*`; 4,349 tensors, BF16 + 290 F32 scale-shift tables, `model_version 2.5.0`, `gemma_source_checkpoint: gemma4-12b-ltx-v1`). Two-pass bake over the **LTX-2.5 dev** base: **PASS 1** = 10Eros style LoRA (rank 512, α 512) at **0.85** on the style layers; **PASS 2** = a rank-256 LoRA on the **audio** branch only (0.85 audio / 0 elsewhere — hence `audio_r256_rest_0`). The `_SULPHUR` builds swap the PASS-2 LoRA for `Sulphur_r256`.

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **2.3** | distilled-baked 10Eros + Sulphur style | `v1 r256` | ![bf16][badge-bf16] | 46.14 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.3_DISTILLED_BAKED_LTX_SULPHUR_STYLE_IS_10Eros_v1_r256.safetensors) |
| **2.3** | distilled-baked 10Eros + Sulphur style | `v1 r512` | ![bf16][badge-bf16] | 46.14 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.3_DISTILLED_BAKED_LTX_SULPHUR_STYLE_IS_10Eros_v1_r512.safetensors) |
| **2.3** | distilled-baked 10Eros + Sulphur style | `v12 r256` | ![bf16][badge-bf16] | 46.14 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.3_DISTILLED_BAKED_LTX_SULPHUR_STYLE_IS_10Eros_v12_r256.safetensors) |
| **2.3** | distilled-baked 10Eros + Sulphur style | `v12 r512` | ![bf16][badge-bf16] | 46.14 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.3_DISTILLED_BAKED_LTX_SULPHUR_STYLE_IS_10Eros_v12_r512.safetensors) |
| **2.3** | distilled-baked 10Eros + Sulphur style | `v13 r256` | ![bf16][badge-bf16] | 46.14 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.3_DISTILLED_BAKED_LTX_SULPHUR_STYLE_IS_10Eros_v13_r256.safetensors) |
| **2.3** | distilled-baked 10Eros + Sulphur style | `v13 r512` | ![bf16][badge-bf16] | 46.14 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.3_DISTILLED_BAKED_LTX_SULPHUR_STYLE_IS_10Eros_v13_r512.safetensors) |
| **2.3** | distilled-baked 10Eros + Sulphur style | `v14 r256` | ![bf16][badge-bf16] | 46.14 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.3_DISTILLED_BAKED_LTX_SULPHUR_STYLE_IS_10Eros_v14_r256.safetensors) |
| **2.3** | distilled-baked 10Eros + Sulphur style | `v14 r512` | ![bf16][badge-bf16] | 46.14 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.3_DISTILLED_BAKED_LTX_SULPHUR_STYLE_IS_10Eros_v14_r512.safetensors) |
| **2.3** | distilled-baked 10Eros + Sulphur style | `v15 r256` | ![bf16][badge-bf16] | 46.14 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.3_DISTILLED_BAKED_LTX_SULPHUR_STYLE_IS_10Eros_v15_r256.safetensors) |
| **2.3** | distilled-baked 10Eros + Sulphur style | `v15 r512` | ![bf16][badge-bf16] | 46.14 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.3_DISTILLED_BAKED_LTX_SULPHUR_STYLE_IS_10Eros_v15_r512.safetensors) |
| **2.5** | distilled-baked 10Eros style (dev 0.85) | `v1 r512 + audio r256` | ![bf16][badge-bf16] | 42.02 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.5_DISTILLED_STYLE_10Eros_1_r512_audio_r256_rest_0.safetensors) |
| **2.5** | distilled-baked 10Eros style (dev 0.85) | `v12 r512 + audio r256` | ![bf16][badge-bf16] | 42.02 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.5_DISTILLED_STYLE_10Eros_12_r512_audio_r256_rest_0.safetensors) |
| **2.5** | distilled-baked 10Eros style (dev 0.85) | `v13 r512 + audio r256` | ![bf16][badge-bf16] | 42.02 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.5_DISTILLED_STYLE_10Eros_13_r512_audio_r256_rest_0.safetensors) |
| **2.5** | distilled-baked 10Eros style (dev 0.85) | `v14 r512 + audio r256` | ![bf16][badge-bf16] | 42.02 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.5_DISTILLED_STYLE_10Eros_14_r512_audio_r256_rest_0.safetensors) |
| **2.5** | distilled-baked 10Eros style (dev 0.85) | `v15 r512 + audio r256` | ![bf16][badge-bf16] | 42.02 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.5_DISTILLED_STYLE_10Eros_15_r512_audio_r256_rest_0.safetensors) |
| **2.5** | distilled-baked 10Eros + Sulphur style (dev 0.85) | `v1 r512 + audio r256` | ![bf16][badge-bf16] | 42.02 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.5_DISTILLED_STYLE_10Eros_1_SULPHUR_r512_audio_r256_rest_0.safetensors) |
| **2.5** | distilled-baked 10Eros + Sulphur style (dev 0.85) | `v12 r512 + audio r256` | ![bf16][badge-bf16] | 42.02 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.5_DISTILLED_STYLE_10Eros_12_SULPHUR_r512_audio_r256_rest_0.safetensors) |
| **2.5** | distilled-baked 10Eros + Sulphur style (dev 0.85) | `v13 r512 + audio r256` | ![bf16][badge-bf16] | 42.02 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.5_DISTILLED_STYLE_10Eros_13_SULPHUR_r512_audio_r256_rest_0.safetensors) |
| **2.5** | distilled-baked 10Eros + Sulphur style (dev 0.85) | `v14 r512 + audio r256` | ![bf16][badge-bf16] | 42.02 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.5_DISTILLED_STYLE_10Eros_14_SULPHUR_r512_audio_r256_rest_0.safetensors) |
| **2.5** | distilled-baked 10Eros + Sulphur style (dev 0.85) | `v15 r512 + audio r256` | ![bf16][badge-bf16] | 42.02 GB | [![ibyteohdear][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/Lightricks-LTX-2-DISTILLED-10-Eros/resolve/main/LTX2.5_DISTILLED_STYLE_10Eros_15_SULPHUR_r512_audio_r256_rest_0.safetensors) |

<p id="finetune-10eros-max-h3" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ 10Eros Max (MiniMax-H3 grafts)

⚠️ **This is a different architecture — these are *not* LTX-2.3 checkpoints.** `10Eros Max` is a **MiniMax-H3 (Hailuo 3)** model line. The weights are a 50-block H3 transformer (`token_refiner.blocks`, `final_layer.video_out` / `audio_out`, `video_patch_proj`, `audio_patch_proj`, `condition_proj`) with character **cross-model grafted into the attention layers** from **LTX-2.3, Wan 2.2 and Krea 2**. Verified by safetensors header and model card: `base_model: MiniMaxAI/MiniMax-H3`, `image_model: minimax_h3`, `converted_from: diffusers MiniMax-H3 transformer`. The pruned builds are **20.11 B** params; the unpruned `beta6_bf16` is **33.12 B** (535 tensors, all BF16) and carries a `bias` set that the stock H3 base does not.

◦ **Licence:** the standard **MiniMax-H3 community licence** applies. Because the release carries transferred character from LTX 2.3, Wan 2.2 and Krea 2, **those source licences apply too** to the portions of character that came from each.

◦ **Author's method** is documented in [`h3_graft_methodology.md`](https://huggingface.co/TenStrip/10Eros-Max/blob/main/h3_graft_methodology.md) — an unfuse→graft→refuse toolchain that maps donor attention heads and MLP inner dimensions onto H3's decomposition (Krea 2's 6144 hidden is truncated to H3's 5376; Wan 2.2's biases are discarded because H3 is bias-free).

◦ **Sampling:** `res_multistep` / `simple` at 6–8 steps gives the best motion; `LCM` / `simple` at 6–8 steps the best turbo audio; `er_sde` at 4–6 steps. **Avoid SLA sparsity — it destroys these weights.** "Turbo" builds bake the 4-step turbo delta in (saves ~4.2 GB of VRAM); a 4-step turbo LoRA can be stacked on a reference build to reach 4 steps. Per the author, **beta_3 and beta_4 are corrupted test versions** and **beta_5 is the first fully functional one**.

◦ **Do not confuse with the LTX-2.3 `10Eros` line** in the table above — those are true `AVTransformer3DModel` LTX-2.3 checkpoints.

**Public weights — [`TenStrip/10Eros-Max`](https://huggingface.co/TenStrip/10Eros-Max)** (17 checkpoints + 1 LoRA):

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **H3** | beta6 — 8-step TURBO, unpruned | `10Eros_Max_h3_8stepTURBO_beta6_bf16` | ![bf16][badge-bf16] | 66.25 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_8stepTURBO_beta6_bf16.safetensors) |
| **H3** | beta6 — 8-step TURBO, pruned | `10Eros_Max_h3_8stepTURBO_beta6_pruned` | ![bf16][badge-bf16] | 40.22 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_8stepTURBO_beta6_pruned.safetensors) |
| **H3** | beta6 — 8-step TURBO, pruned | `10Eros_Max_h3_8stepTURBO_beta6_int8` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 21.71 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_8stepTURBO_beta6_int8.safetensors) |
| **H3** | beta6 — VSA gates (unstable) | `10Eros_Max_FastH3_VSAgates_UNSTABLE_beta6-int8_HQ` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 26.75 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_FastH3_VSAgates_UNSTABLE_beta6-int8_HQ.safetensors) |
| **H3** | beta5 — TURBO hybrid | `10Eros_Max_h3_TURBO-hybrid_beta5` | ![bf16][badge-bf16] | 40.22 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_TURBO-hybrid_beta5.safetensors) |
| **H3** | beta5 — TURBO hybrid | `10Eros_Max_h3_TURBO-hybrid_beta5_int8` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 20.97 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_TURBO-hybrid_beta5_int8.safetensors) |
| **H3** | beta5 — TURBO hybrid, 14 GB opt | `10Eros_Max_h3_TURBO-hybrid_beta5_w4a8_14gb_optimized` | ![w4a8](https://img.shields.io/badge/w4a8-17a2b8?style=flat-square) | 14.00 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_TURBO-hybrid_beta5_w4a8_14gb_optimized.safetensors) |
| **H3** | beta5 — hybrid (non-turbo) | `10Eros_Max_h3_hybrid_beta5` | ![bf16][badge-bf16] | 40.22 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_hybrid_beta5.safetensors) |
| **H3** | beta5 — hybrid (non-turbo) | `10Eros_Max_h3_hybrid_beta5_int8` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 20.97 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_hybrid_beta5_int8.safetensors) |
| **H3** | beta5 — hybrid, 14 GB opt | `10Eros_Max_h3_hybrid_beta5_w4a8_14gb_optimized` | ![w4a8](https://img.shields.io/badge/w4a8-17a2b8?style=flat-square) | 14.00 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_hybrid_beta5_w4a8_14gb_optimized.safetensors) |
| **H3** | beta3 — TURBO hybrid (corrupted test) | `10Eros_Max_h3_TURBO-hybrid_beta3` | ![bf16][badge-bf16] | 40.23 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_TURBO-hybrid_beta3.safetensors) |
| **H3** | beta3 — TURBO hybrid (corrupted test) | `10Eros_Max_h3_TURBO-hybrid_beta3_int8_convrot` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 20.98 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_TURBO-hybrid_beta3_int8_convrot.safetensors) |
| **H3** | beta4 — TURBO hybrid (corrupted test) | `10Eros_Max_h3_TURBO-hybrid_beta4` | ![bf16][badge-bf16] | 40.22 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_TURBO-hybrid_beta4.safetensors) |
| **H3** | beta4 — TURBO hybrid (corrupted test) | `10Eros_Max_h3_TURBO-hybrid_beta4_int8_convrot` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 20.97 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_TURBO-hybrid_beta4_int8_convrot.safetensors) |
| **H3** | beta2 — ref2va, TURBO | `10Eros_Max_h3_TURBO_ref2va_beta2` | ![bf16][badge-bf16] | 40.23 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_TURBO_ref2va_beta2.safetensors) |
| **H3** | beta2 — ref2va, pruned | `10Eros_Max_h3_ref2va_beta2_pruned` | ![bf16][badge-bf16] | 40.22 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_ref2va_beta2_pruned.safetensors) |
| **H3** | beta2 — fl2va, pruned | `10Eros_Max_h3_fl2va_beta2_pruned` | ![bf16][badge-bf16] | 40.22 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/10Eros_Max_h3_fl2va_beta2_pruned.safetensors) |

<details>
  <summary>Gated beta7 set — <code>TenStrip/LTX2.3-10Eros_Version-Testing</code> (18 weights, 476.55 GB)</summary>

[`TenStrip/LTX2.3-10Eros_Version-Testing`](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing) is **gated `manual`** — request access, it is not instant auto-approve, and the model card itself is locked. The repo was **fully replaced on 2026-10-27**: every `beta6` file the README previously linked to is gone, and the tree now holds only `beta7` weights (plus a 626-byte README). File names and byte sizes below come from the public tree API; **precision labels are inferred from the file names** because a gated checkpoint's header cannot be fetched without approval.

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **H3** | beta7 test1 — 8-step TURBO | `10Eros_Max_h3_8stepTURBO_beta7_test1` | ![bf16][badge-bf16] | 40.22 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_8stepTURBO_beta7_test1.safetensors) |
| **H3** | beta7 test1 — 8-step TURBO | `10Eros_Max_h3_8stepTURBO_beta7_test1-int8` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 20.97 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_8stepTURBO_beta7_test1-int8.safetensors) |
| **H3** | beta7 test1 — 8-step TURBO | `10Eros_Max_h3_8stepTURBO_beta7_test1-int8_HQ` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 24.63 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_8stepTURBO_beta7_test1-int8_HQ.safetensors) |
| **H3** | beta7 test1 — 8-step TURBO | `10Eros_Max_h3_8stepTURBO_beta7_test1-int8_learned` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 20.97 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_8stepTURBO_beta7_test1-int8_learned.safetensors) |
| **H3** | beta7 test1 — 8-step TURBO | `10Eros_Max_h3_8stepTURBO_beta7_test1-w4a8_conservative_cicalooo` | ![w4a8](https://img.shields.io/badge/w4a8-17a2b8?style=flat-square) | 19.08 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_8stepTURBO_beta7_test1-w4a8_conservative_cicalooo.safetensors) |
| **H3** | beta7 test1 — 8-step TURBO | `10Eros_Max_h3_8stepTURBO_beta7_test1_activation_learned_HQ` | ![fp8](https://img.shields.io/badge/fp8-17a2b8?style=flat-square) | 18.69 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_8stepTURBO_beta7_test1_activation_learned_HQ.safetensors) |
| **H3** | beta7 test2 — 8-step TURBO | `10Eros_Max_h3_8stepTURBO_beta7_test2` | ![bf16][badge-bf16] | 40.22 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_8stepTURBO_beta7_test2.safetensors) |
| **H3** | beta7 test2 — 8-step TURBO | `10Eros_Max_h3_8stepTURBO_beta7_test2-int8` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 20.97 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_8stepTURBO_beta7_test2-int8.safetensors) |
| **H3** | beta7 test2 — 8-step TURBO | `10Eros_Max_h3_8stepTURBO_beta7_test2-native_int8_HQ` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 22.89 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_8stepTURBO_beta7_test2-native_int8_HQ.safetensors) |
| **H3** | beta7 test2 — 8-step TURBO | `10Eros_Max_h3_8stepTURBO_beta7_test2_activation_learned_HQ` | ![fp8](https://img.shields.io/badge/fp8-17a2b8?style=flat-square) | 18.69 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_8stepTURBO_beta7_test2_activation_learned_HQ.safetensors) |
| **H3** | beta7 test2 — 8-step TURBO | `10Eros_Max_h3_8stepTURBO_beta7_test2_cicaloo_w4a8conservative_gptq_activated` | ![w4a8](https://img.shields.io/badge/w4a8-17a2b8?style=flat-square) | 19.08 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_8stepTURBO_beta7_test2_cicaloo_w4a8conservative_gptq_activated.safetensors) |
| **H3** | beta7 test3 — 8-step TURBO | `10Eros_Max_h3_8stepTURBO_beta7_test3` | ![bf16][badge-bf16] | 40.22 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_8stepTURBO_beta7_test3.safetensors) |
| **H3** | beta7 test3 — 8-step TURBO | `10Eros_Max_h3_8stepTURBO_beta7_test3-native_int8_protected_edges_HQ` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 22.89 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_8stepTURBO_beta7_test3-native_int8_protected_edges_HQ.safetensors) |
| **H3** | beta7 test1 — raw (no turbo) | `10Eros_Max_h3_raw_beta7_test1` | ![bf16][badge-bf16] | 40.22 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_raw_beta7_test1.safetensors) |
| **H3** | beta7 test1 — raw (no turbo) | `10Eros_Max_h3_raw_beta7_test1-int8` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 20.97 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_raw_beta7_test1-int8.safetensors) |
| **H3** | beta7 test1 — raw (no turbo) | `10Eros_Max_h3_raw_beta7_test1-int8_HQ` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 24.63 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_raw_beta7_test1-int8_HQ.safetensors) |
| **H3** | beta7 test2 — raw (no turbo) | `10Eros_Max_h3_raw_beta7_test2` | ![bf16][badge-bf16] | 40.22 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_raw_beta7_test2.safetensors) |
| **H3** | beta7 test2 — raw (no turbo) | `10Eros_Max_h3_raw_beta7_test2-int8` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 20.97 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros_Version-Testing/resolve/main/10Eros_Max_h3_raw_beta7_test2-int8.safetensors) |

</details>

<details>
  <summary>int8 ConvRot mirrors — <code>cicalooo/10Eros-Max-h3-int8-convrot</code> + <code>CornLogic/10EROS-INT8</code></summary>

The int8 ConvRot H3 builds are mirrored publicly. `cicalooo`'s `_skip_edges` variants keep the **first and last blocks in BF16** (see the repo's `SKIP_EDGES.md`) — use them when ConvRot rotation hurts the edge blocks.

**[`cicalooo/10Eros-Max-h3-int8-convrot`](https://huggingface.co/cicalooo/10Eros-Max-h3-int8-convrot)** (8 files, 172.38 GB):

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **H3** | beta3 — TURBO hybrid | `10Eros_Max_h3_TURBO-hybrid_beta3_int8_convrot` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 20.97 GB | [![cicalooo][gh-cicalooo]](https://huggingface.co/cicalooo/10Eros-Max-h3-int8-convrot/resolve/main/10Eros_Max_h3_TURBO-hybrid_beta3_int8_convrot.safetensors) |
| **H3** | beta3 — TURBO hybrid, skip edges | `10Eros_Max_h3_TURBO-hybrid_beta3_int8_convrot_skip_edges` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 22.51 GB | [![cicalooo][gh-cicalooo]](https://huggingface.co/cicalooo/10Eros-Max-h3-int8-convrot/resolve/main/10Eros_Max_h3_TURBO-hybrid_beta3_int8_convrot_skip_edges.safetensors) |
| **H3** | beta2 — ref2va | `10Eros_Max_h3_TURBO_ref2va_beta2_int8_convrot` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 20.97 GB | [![cicalooo][gh-cicalooo]](https://huggingface.co/cicalooo/10Eros-Max-h3-int8-convrot/resolve/main/10Eros_Max_h3_TURBO_ref2va_beta2_int8_convrot.safetensors) |
| **H3** | beta2 — ref2va, skip edges | `10Eros_Max_h3_TURBO_ref2va_beta2_int8_convrot_skip_edges` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 22.51 GB | [![cicalooo][gh-cicalooo]](https://huggingface.co/cicalooo/10Eros-Max-h3-int8-convrot/resolve/main/10Eros_Max_h3_TURBO_ref2va_beta2_int8_convrot_skip_edges.safetensors) |
| **H3** | beta2 — fl2va, pruned | `10Eros_Max_h3_fl2va_beta2_pruned_int8_convrot` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 20.20 GB | [![cicalooo][gh-cicalooo]](https://huggingface.co/cicalooo/10Eros-Max-h3-int8-convrot/resolve/main/10Eros_Max_h3_fl2va_beta2_pruned_int8_convrot.safetensors) |
| **H3** | beta2 — fl2va, pruned, skip edges | `10Eros_Max_h3_fl2va_beta2_pruned_int8_convrot_skip_edges` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 21.74 GB | [![cicalooo][gh-cicalooo]](https://huggingface.co/cicalooo/10Eros-Max-h3-int8-convrot/resolve/main/10Eros_Max_h3_fl2va_beta2_pruned_int8_convrot_skip_edges.safetensors) |
| **H3** | beta2 — ref2va, pruned | `10Eros_Max_h3_ref2va_beta2_pruned_int8_convrot` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 20.97 GB | [![cicalooo][gh-cicalooo]](https://huggingface.co/cicalooo/10Eros-Max-h3-int8-convrot/resolve/main/10Eros_Max_h3_ref2va_beta2_pruned_int8_convrot.safetensors) |
| **H3** | beta2 — ref2va, pruned, skip edges | `10Eros_Max_h3_ref2va_beta2_pruned_int8_convrot_skip_edges` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 22.51 GB | [![cicalooo][gh-cicalooo]](https://huggingface.co/cicalooo/10Eros-Max-h3-int8-convrot/resolve/main/10Eros_Max_h3_ref2va_beta2_pruned_int8_convrot_skip_edges.safetensors) |

**[`CornLogic/10EROS-INT8`](https://huggingface.co/CornLogic/10EROS-INT8)** — H3 int8 files only (the repo's LTX-2.3 v1.5 files are listed in the [`❖ 10Eros`](#finetune-10eros) table above):

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **H3** | beta1 — fl2va, pruned | `10Eros_Max_h3_fl2va_INT8_beta1_pruned` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 20.97 GB | [![CornLogic][gh-CornLogic]](https://huggingface.co/CornLogic/10EROS-INT8/resolve/main/10Eros_Max_h3_fl2va_INT8_beta1_pruned.safetensors) |
| **H3** | test2 — fl2va, pruned | `10Eros_Max_h3_fl2va_INT8_test2_pruned` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 20.97 GB | [![CornLogic][gh-CornLogic]](https://huggingface.co/CornLogic/10EROS-INT8/resolve/main/10Eros_Max_h3_fl2va_INT8_test2_pruned.safetensors) |
| **H3** | test4 — fl2va, pruned | `10Eros_Max_h3_fl2va_INT8_test4_pruned` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 20.97 GB | [![CornLogic][gh-CornLogic]](https://huggingface.co/CornLogic/10EROS-INT8/resolve/main/10Eros_Max_h3_fl2va_INT8_test4_pruned.safetensors) |

</details>

**H3 LoRAs** — these target the **MiniMax-H3** transformer, **not** an LTX DiT, so they will not load into any LTX checkpoint. They are listed here with the H3 line rather than in the LTX LoRA tables of block 60.

| LoRA | Ver | Size | Description | Download |
| :--- | :---: | :---: | :--- | :--- |
| `Eros_beta6mix_Lora` | H3 | 387.63 MB | Rank-32 H3 PEFT LoRA for the 10Eros Max beta6 line — a `dare_ties` merge of 17 satellite LoRAs (ties density 0.3, sign consensus mass) | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/10Eros-Max/resolve/main/Loras/Eros_beta6mix_Lora.safetensors) |
| `H3_krea_style_test1_rank512` | H3 | 1.10 GB | Krea-2 style LoRA extracted from the Krea-2 branch of the author's attn-graft experiments (rank 512 captures ~52% of the SLERP orthogonal delta). **T2V only.** | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/Krea2-H3-Style-Lora/resolve/main/H3_krea_style_test1_rank512.safetensors) |
| `H3_krea_style_test1_rank128` | H3 | 275.27 MB | Same as above at rank 128 (~24% of the delta — small but visibly shifts visual style) | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/Krea2-H3-Style-Lora/resolve/main/H3_krea_style_test1_rank128.safetensors) |
| `H3_Anima_Tokenizer` | H3 | 763.37 MB | Anima-style LoRA grafted across the H3 **text-encoder** layers of token-refiner blocks 0–1, extracted at rank 2048. Strongly affects style in T2V and detail in I2V | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/Anima-H3-Booster-Lora/resolve/main/H3_Anima_Tokenizer.safetensors) |
| `Minimax-h3_Singularity_128spect-fro95_lora` | H3 | 1.28 GB | Extracted from the base hybrid pruned build with spectral dampening, against [WarmBloodAban/Minimax-h3_Singularity](https://huggingface.co/WarmBloodAban/Minimax-h3_Singularity). **Use at 0.5 strength or lower** — higher strengths can drift | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/Minimax-h3_Singularity-Lora/resolve/main/Minimax-h3_Singularity_128spect-fro95_lora.safetensors) |
| `Minimax-h3_Singularity_64-fro95_lora` | H3 | 655.31 MB | Same as above at rank 64 | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/Minimax-h3_Singularity-Lora/resolve/main/Minimax-h3_Singularity_64-fro95_lora.safetensors) |
| `H3_Wan2.2_i2v_motion_rank1024_test1` | H3 | 1.38 GB | Wan-2.2 motion LoRA grafted onto the mid-to-late H3 blocks with peak mapping (rank 1024 captures ~69% of the residual delta). Shifts motion style towards Wan's repetitive motion | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/Wan2.2_H3_Motion_Lora/resolve/main/H3_Wan2.2_i2v_motion_rank1024_test1.safetensors) |
| `H3_Wan2.2_i2v_motion_rank512_test1` | H3 | 688.14 MB | Same as above at rank 512 (~41.6% of the residual delta) | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/Wan2.2_H3_Motion_Lora/resolve/main/H3_Wan2.2_i2v_motion_rank512_test1.safetensors) |
| `lightx2v_hybrid-4to8step-Turbo_r48` | H3 | 943.95 MB | H3 PEFT turbo LoRA turning 8-step sampling into 4-step (rank 48) | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/MinimaxH3-Turbo_Shenanigans/resolve/main/lightx2v_hybrid-4to8step-Turbo_r48.safetensors) |
| `lightx2v_hybrid-4to8step-full-fusion_Turbo_pruned` | H3 | 4.46 GB | Full-fusion H3 turbo build (777 tensors: 750 `diffusion_model.blocks` + 24 `token_refiner` + 3 `final_layer`) — loads standalone instead of as a LoRA | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/MinimaxH3-Turbo_Shenanigans/resolve/main/lightx2v_hybrid-4to8step-full-fusion_Turbo_pruned.safetensors) |

<p id="finetune-sulphur" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ Sulphur-2-base

Repo: [`SulphurAI/Sulphur-2-base`](https://huggingface.co/SulphurAI/Sulphur-2-base) — uncensored video generation model based on LTX 2.3 with built-in prompt enhancer. Merge base for 10Eros. T2V + I2V native.

◦ **Main video model**

| Ver | Build | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.3** | dev | ![bf16][badge-bf16] | 46.14 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/sulphur_dev_bf16.safetensors) |
| **2.3** | dev | ![fp8][badge-fp8] | 29.16 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/sulphur_dev_fp8mixed.safetensors) |
| **2.3** | distil | ![bf16][badge-bf16] | 46.14 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/sulphur_distil_bf16.safetensors) |
| **2.3** | distil | ![fp8][badge-fp8] | 29.16 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/Civitai/Sulphur-2-distilled-fp8/resolve/main/sulphur_distil_fp8mixed.safetensors) |
| **2.3** | distil | ![nvfp4][badge-nvfp4] | 19.51 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/coolthor/Sulphur-2-distilled-NVFP4/resolve/main/sulphur_distil_nvfp4.safetensors) |

◦ **vantagewithai component split** — [`vantagewithai/Sulphur-2-Base-Split`](https://huggingface.co/vantagewithai/Sulphur-2-Base-Split)

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| model (`sulphur_dev_bf16_model`) | ![bf16][badge-bf16] | 42.01 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/Sulphur-2-Base-Split/resolve/main/model/sulphur_dev_bf16_model.safetensors) |
| model (`sulphur_dev_model_fp8mixed`) | ![fp8][badge-fp8] | 25.03 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/Sulphur-2-Base-Split/resolve/main/model/sulphur_dev_model_fp8mixed.safetensors) |
| model (`sulphur_distil_bf16_model`) | ![bf16][badge-bf16] | 42.01 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/Sulphur-2-Base-Split/resolve/main/model/sulphur_distil_bf16_model.safetensors) |
| vae | — | 1.45 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/Sulphur-2-Base-Split/resolve/main/vae/sulphur_vae.safetensors) |
| audio_vae | — | 364.86 MB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/Sulphur-2-Base-Split/resolve/main/audio_vae/sulphur_audio_vae.safetensors) |

<details>
  <summary>Abiray GGUF quants</summary>

◦ **Abiray GGUF quants** — [`Abiray/Sulphur-2-base-GGUF`](https://huggingface.co/Abiray/Sulphur-2-base-GGUF)

| Build | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| sulphur_dev | ![bf16][badge-bf16] | 42.03 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev_bf16.gguf) |
| sulphur_dev | ![Q3_K_M][badge-Q3_K_M] | 11.13 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q3_K_M.gguf) |
| sulphur_dev | ![Q3_K_S][badge-Q3_K_S] | 10.34 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q3_K_S.gguf) |
| sulphur_dev | ![Q4_0][badge-Q4_0] | 12.98 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q4_0.gguf) |
| sulphur_dev | ![Q4_K_M][badge-Q4_K_M] | 14.3 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q4_K_M.gguf) |
| sulphur_dev | ![Q4_K_S][badge-Q4_K_S] | 13.2 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q4_K_S.gguf) |
| sulphur_dev | ![Q5_0][badge-Q5_0] | 15.26 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q5_0.gguf) |
| sulphur_dev | ![Q5_K_M][badge-Q5_K_M] | 16.14 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q5_K_M.gguf) |
| sulphur_dev | ![Q5_K_S][badge-Q5_K_S] | 15.04 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q5_K_S.gguf) |
| sulphur_dev | ![Q6_K][badge-Q6_K] | 17.77 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q6_K.gguf) |
| sulphur_dev | ![Q8_0][badge-Q8_0] | 22.76 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q8_0.gguf) |


</details>

◦ **Sulphur LoRAs**

| Ver | Build | Size | Download |
| :--- | :--- | :---: | :---: |
| **2.3** | `sulphur_lora_rank_768` | 10.27 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/sulphur_lora_rank_768.safetensors) |
| **2.3** (experimental) | `sulphur_experimental_lora_v1` | 14.54 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/experimental/sulphur_experimental_lora_v1.safetensors) |

◦ **Prompt Enhancer**

| Variant | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| Censored | ![bf16][badge-bf16] | 921.71 MB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/prompt_enhancer/mmproj-BF16.gguf) ┆ [![][gh-EllaPriest45]](https://huggingface.co/EllaPriest45/LTX2.3_base/resolve/main/Text%20encoder%20-%20Mmproj-BF16.gguf) |
| Censored | ![Q8_0][badge-Q8_0] | 9.53 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/prompt_enhancer/sulphur_prompt_enhancer_model-q8_0.gguf) ┆ [![][gh-EllaPriest45]](https://huggingface.co/EllaPriest45/LTX2.3_base/resolve/main/Text%20encoder%20-%20Qwen3.5-sulphur_prompt_enhancer-Q8_0.gguf) |
| Uncensored | ![bf16][badge-bf16] | 921.7 MB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/prompt_enhancer_uncensored/mmproj-prompt_enhancer_uncensored.gguf) ┆ [![][gh-EllaPriest45]](https://huggingface.co/EllaPriest45/LTX2.3_base/resolve/main/Sulphur2promptenhancer_mmproj-prompt_enhancer_uncensored.gguf) |
| Uncensored | ![Q8_0][badge-Q8_0] | 9.79 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/prompt_enhancer_uncensored/prompt_enhancer_uncensored-q8_0.gguf) ┆ [![][gh-EllaPriest45]](https://huggingface.co/EllaPriest45/LTX2.3_base/resolve/main/Sulphur2promptenhancer_prompt_enhancer_uncensored-q8_0.gguf) |
| Uncensored (safetensors) | ![bf16][badge-bf16] | 19.31 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/prompt_enhancer_uncensored/model.safetensors.index.json) |

◦ The uncensored prompt enhancer also ships as a **4-shard safetensors** set (19.31 GB total) next to the Q8_0 GGUF — download `model.safetensors.index.json` and the four `model.safetensors-0000N-of-00004.safetensors` shards it names (the tokenizer / processor / chat-template JSONs sit alongside them). The four `EllaPriest45/LTX2.3_base` copies are **byte-identical re-packs** of the official files (matching byte counts), listed as second links above.

<p id="finetune-joyai-echo-surgical" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ JoyAI-Echo Surgical

Surgical finetune based on [jdopensource/JoyAI-Echo](https://huggingface.co/jdopensource/JoyAI-Echo) by joeygambino. Combined "echoVid + ltxAud" surgical variant — jointly fine-tuned for both video generation and audio on top of LTX-2.3. A LoRA extracted from JoyAI-Echo (TenStrip's `LTX2.3_JoyAI_Lora_Extracted`) is listed separately under `### ▣ Special`.

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **2.3** | unsplit (full DiT) | `echoVid-ltxAud surgical` | ![bf16][badge-bf16] | 46.14 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical/resolve/main/ltx23_echoVid-ltxAud_surgical_bf16.safetensors) |
| **2.3** | unsplit (full DiT) | `echoVid-ltxAud surgical` | ![fp8][badge-fp8] | 25.13 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical/resolve/main/ltx23_echoVid-ltxAud_surgical_fp8.safetensors) |
| **2.3** | unsplit (full DiT) | `echoVid-ltxAud surgical` | ![int8tensormixed][badge-int8tensormixed] | 29.16 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical-int8/resolve/main/ltx23_echoVid-ltxAud_surgical_int8_convrot.safetensors) |
| **2.3** | transformer-only | `echoVid-ltxAud surgical` | ![int8tensormixed][badge-int8tensormixed] | 27.34 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical-int8/resolve/main/ltx23_echoVid-ltxAud_surgical_int8_convrot_transformer_only.safetensors) |

◦ **JoyAI-Echo Surgical — GGUF (low-VRAM quants)**

<details>
  <summary>joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical-gguf</summary>

[`joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical-gguf`](https://huggingface.co/joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical-gguf) — Surgical DiT GGUF quants by joeygambino.

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **2.3** | GGUF | `echoVid-ltxAud surgical` | ![Q5_0][badge-Q5_0] | 16.69 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical-gguf/resolve/main/LTX23-echoVid-ltxAud-Surgical-DiT-Q5_0.gguf) |
| **2.3** | GGUF | `echoVid-ltxAud surgical` | ![Q8_0][badge-Q8_0] | 24.83 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical-gguf/resolve/main/LTX23-echoVid-ltxAud-Surgical-DiT-Q8_0.gguf) |

</details>

<p id="finetune-joyai-echo-ltx25" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ JoyAI-Echo (LTX-2.5)

Surgical merge of [jdopensource/JoyAI-Echo](https://huggingface.co/jdopensource/JoyAI-Echo) into the **LTX-2.5** `dev` transformer by joeygambino — JoyAI-Echo's video attention / feed-forward delta transplanted in, with nothing distilled baked on top. Three builds: `dev` (bring-your-own distill LoRA), `comfy-native` (few-step, distill baked at 0.5 — RTX 50), and GGUF (few-step — RTX 30/40). Two doses per build: `070T30` (0.7× delta / 0.3× modulation) and `100T50` (1.0× / 0.5×). Workflows: [ComfyUI-JoyLTX25](https://github.com/jlucasmcrell/ComfyUI-JoyLTX25).

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **2.5** | dev | `echoVid 070T30` | ![bf16][badge-bf16] | 42.02 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-dev/resolve/main/LTX25dev-echoVid-070T30-DiT-bf16.safetensors) |
| **2.5** | dev | `echoVid 070T30` | ![fp8][badge-fp8] | 21.48 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-dev/resolve/main/LTX25dev-echoVid-070T30-DiT-comfy-fp8.safetensors) |
| **2.5** | dev | `echoVid 070T30` | ![int8tensormixed][badge-int8tensormixed] | 21.50 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-dev/resolve/main/LTX25dev-echoVid-070T30-DiT-comfy-int8.safetensors) |
| **2.5** | dev | `echoVid 100T50` | ![bf16][badge-bf16] | 42.02 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-dev/resolve/main/LTX25dev-echoVid-100T50-DiT-bf16.safetensors) |
| **2.5** | dev | `echoVid 100T50` | ![fp8][badge-fp8] | 21.48 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-dev/resolve/main/LTX25dev-echoVid-100T50-DiT-comfy-fp8.safetensors) |
| **2.5** | dev | `echoVid 100T50` | ![int8tensormixed][badge-int8tensormixed] | 21.50 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-dev/resolve/main/LTX25dev-echoVid-100T50-DiT-comfy-int8.safetensors) |
| **2.5** | comfy-native | `echoVid 070T30` | ![int8tensormixed][badge-int8tensormixed] | 21.50 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-comfy-native/resolve/main/LTX25dist-echoVid-070T30-v2-DiT-comfy-int8.safetensors) |
| **2.5** | comfy-native | `echoVid 070T30` | ![mix4x8](https://img.shields.io/badge/mix4x8-17a2b8?style=flat-square) | 17.01 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-comfy-native/resolve/main/LTX25dist-echoVid-070T30-v2-DiT-comfy-mix4x8-17.0GB.safetensors) |
| **2.5** | comfy-native | `echoVid 070T30` | ![nvfp4][badge-nvfp4] | 12.50 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-comfy-native/resolve/main/LTX25dist-echoVid-070T30-v2-DiT-comfy-nvfp4.safetensors) |
| **2.5** | comfy-native | `echoVid 070T30` | ![w4a4](https://img.shields.io/badge/w4a4-17a2b8?style=flat-square) | 11.24 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-comfy-native/resolve/main/LTX25dist-echoVid-070T30-v2-DiT-comfy-w4a4.safetensors) |
| **2.5** | comfy-native | `echoVid 070T30` | ![w4a8](https://img.shields.io/badge/w4a8-17a2b8?style=flat-square) | 12.52 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-comfy-native/resolve/main/LTX25dist-echoVid-070T30-v2-DiT-comfy-w4a8.safetensors) |
| **2.5** | comfy-native | `echoVid 100T50` | ![int8tensormixed][badge-int8tensormixed] | 21.50 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-comfy-native/resolve/main/LTX25dist-echoVid-100T50-v2-DiT-comfy-int8.safetensors) |
| **2.5** | comfy-native | `echoVid 100T50` | ![mix4x8](https://img.shields.io/badge/mix4x8-17a2b8?style=flat-square) | 13.81 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-comfy-native/resolve/main/LTX25dist-echoVid-100T50-v2-DiT-comfy-mix4x8-13.8GB.safetensors) |
| **2.5** | comfy-native | `echoVid 100T50` | ![mix4x8](https://img.shields.io/badge/mix4x8-17a2b8?style=flat-square) | 17.01 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-comfy-native/resolve/main/LTX25dist-echoVid-100T50-v2-DiT-comfy-mix4x8-17.0GB.safetensors) |
| **2.5** | comfy-native | `echoVid 100T50` | ![nvfp4][badge-nvfp4] | 12.50 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-comfy-native/resolve/main/LTX25dist-echoVid-100T50-v2-DiT-comfy-nvfp4.safetensors) |
| **2.5** | comfy-native | `echoVid 100T50` | ![w4a4](https://img.shields.io/badge/w4a4-17a2b8?style=flat-square) | 11.24 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-comfy-native/resolve/main/LTX25dist-echoVid-100T50-v2-DiT-comfy-w4a4.safetensors) |
| **2.5** | comfy-native | `echoVid 100T50` | ![w4a8](https://img.shields.io/badge/w4a8-17a2b8?style=flat-square) | 12.52 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-comfy-native/resolve/main/LTX25dist-echoVid-100T50-v2-DiT-comfy-w4a8.safetensors) |

**Z-Image surface-graft variant (`× Z-Image`)** — same `echoVid 070T30 v2` engine with [Z-Image](https://huggingface.co/Tongyi-MAI/Z-Image)'s spatial attention profile grafted in as per-block `q_norm` rescaling (dose 0.5, no retraining, no Z-Image weights at inference). Targets surface/texture rendering: fine detail on foliage, straw, gravel, fabric and skin. Drop-in replacement for any stock v2 workflow — same loaders, settings and seeds.

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **2.5** | comfy-native | `echoVid 070T30 × Z-Image zgraft05` | ![bf16][badge-bf16] | 42.02 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-native/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-bf16.safetensors) |
| **2.5** | comfy-native | `echoVid 070T30 × Z-Image zgraft05` | ![fp8][badge-fp8] | 21.48 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-native/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-comfy-fp8.safetensors) |
| **2.5** | comfy-native | `echoVid 070T30 × Z-Image zgraft05` | ![int8tensormixed][badge-int8tensormixed] | 21.50 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-native/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-comfy-int8.safetensors) |
| **2.5** | comfy-native | `echoVid 070T30 × Z-Image zgraft05` | ![mix4x8](https://img.shields.io/badge/mix4x8-17a2b8?style=flat-square) | 13.81 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-native/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-comfy-mix4x8-13.8GB.safetensors) |
| **2.5** | comfy-native | `echoVid 070T30 × Z-Image zgraft05` | ![mix4x8](https://img.shields.io/badge/mix4x8-17a2b8?style=flat-square) | 17.01 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-native/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-comfy-mix4x8-17.0GB.safetensors) |
| **2.5** | comfy-native | `echoVid 070T30 × Z-Image zgraft05` | ![nvfp4][badge-nvfp4] | 12.50 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-native/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-comfy-nvfp4.safetensors) |
| **2.5** | comfy-native | `echoVid 070T30 × Z-Image zgraft05` | ![w4a4](https://img.shields.io/badge/w4a4-17a2b8?style=flat-square) | 11.24 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-native/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-comfy-w4a4.safetensors) |
| **2.5** | comfy-native | `echoVid 070T30 × Z-Image zgraft05` | ![w4a8](https://img.shields.io/badge/w4a8-17a2b8?style=flat-square) | 12.52 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-native/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-comfy-w4a8.safetensors) |

◦ **JoyAI-Echo × Z-Image — GGUF (RTX 30/40; K-quants run 4–8× faster than emulated 4-bit there)**

<details>
  <summary>joeygambino/joyai-echo-ltx25-x-Z-Image-gguf</summary>

[`joeygambino/joyai-echo-ltx25-x-Z-Image-gguf`](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-gguf) — Z-Image-grafted echoVid `070T30 v2` GGUF quants by joeygambino (Q4_K_M/Q4_K_S are the RTX 30/40 sweet spot).

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **2.5** | GGUF | `echoVid 070T30 × Z-Image zgraft05` | ![Q2_K][badge-Q2_K] | 7.91 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-gguf/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-Q2_K.gguf) |
| **2.5** | GGUF | `echoVid 070T30 × Z-Image zgraft05` | ![Q3_K_M][badge-Q3_K_M] | 10.60 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-gguf/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-Q3_K_M.gguf) |
| **2.5** | GGUF | `echoVid 070T30 × Z-Image zgraft05` | ![Q4_K_M][badge-Q4_K_M] | 14.17 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-gguf/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-Q4_K_M.gguf) |
| **2.5** | GGUF | `echoVid 070T30 × Z-Image zgraft05` | ![Q4_K_S][badge-Q4_K_S] | 12.93 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-gguf/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-Q4_K_S.gguf) |
| **2.5** | GGUF | `echoVid 070T30 × Z-Image zgraft05` | ![Q5_K_M][badge-Q5_K_M] | 15.90 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-gguf/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-Q5_K_M.gguf) |
| **2.5** | GGUF | `echoVid 070T30 × Z-Image zgraft05` | ![Q6_K][badge-Q6_K] | 17.75 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-gguf/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-Q6_K.gguf) |
| **2.5** | GGUF | `echoVid 070T30 × Z-Image zgraft05` | ![Q8_0][badge-Q8_0] | 22.73 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-x-Z-Image-gguf/resolve/main/LTX25dist-echoVid-070T30-v2-zgraft05-DiT-Q8_0.gguf) |

</details>

◦ **JoyAI-Echo (LTX-2.5) — GGUF (low-VRAM quants)**

<details>
  <summary>joeygambino/joyai-echo-ltx25-echoVid-gguf</summary>

[`joeygambino/joyai-echo-ltx25-echoVid-gguf`](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf) — echoVid GGUF quants by joeygambino (few-step, distill baked at 0.5; RTX 30/40).

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **2.5** | GGUF | `echoVid 070T30` | ![Q2_K][badge-Q2_K] | 7.91 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf/resolve/main/LTX25dist-echoVid-070T30-v2-DiT-Q2_K.gguf) |
| **2.5** | GGUF | `echoVid 070T30` | ![Q3_K_M][badge-Q3_K_M] | 10.60 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf/resolve/main/LTX25dist-echoVid-070T30-v2-DiT-Q3_K_M.gguf) |
| **2.5** | GGUF | `echoVid 070T30` | ![Q4_K_M][badge-Q4_K_M] | 14.17 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf/resolve/main/LTX25dist-echoVid-070T30-v2-DiT-Q4_K_M.gguf) |
| **2.5** | GGUF | `echoVid 070T30` | ![Q4_K_S][badge-Q4_K_S] | 12.93 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf/resolve/main/LTX25dist-echoVid-070T30-v2-DiT-Q4_K_S.gguf) |
| **2.5** | GGUF | `echoVid 070T30` | ![Q5_K_M][badge-Q5_K_M] | 15.90 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf/resolve/main/LTX25dist-echoVid-070T30-v2-DiT-Q5_K_M.gguf) |
| **2.5** | GGUF | `echoVid 070T30` | ![Q6_K][badge-Q6_K] | 17.75 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf/resolve/main/LTX25dist-echoVid-070T30-v2-DiT-Q6_K.gguf) |
| **2.5** | GGUF | `echoVid 070T30` | ![Q8_0][badge-Q8_0] | 22.73 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf/resolve/main/LTX25dist-echoVid-070T30-v2-DiT-Q8_0.gguf) |
| **2.5** | GGUF | `echoVid 100T50` | ![Q2_K][badge-Q2_K] | 7.91 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf/resolve/main/LTX25dist-echoVid-100T50-v2-DiT-Q2_K.gguf) |
| **2.5** | GGUF | `echoVid 100T50` | ![Q3_K_M][badge-Q3_K_M] | 10.60 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf/resolve/main/LTX25dist-echoVid-100T50-v2-DiT-Q3_K_M.gguf) |
| **2.5** | GGUF | `echoVid 100T50` | ![Q4_K_M][badge-Q4_K_M] | 14.17 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf/resolve/main/LTX25dist-echoVid-100T50-v2-DiT-Q4_K_M.gguf) |
| **2.5** | GGUF | `echoVid 100T50` | ![Q4_K_S][badge-Q4_K_S] | 12.93 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf/resolve/main/LTX25dist-echoVid-100T50-v2-DiT-Q4_K_S.gguf) |
| **2.5** | GGUF | `echoVid 100T50` | ![Q5_K_M][badge-Q5_K_M] | 15.90 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf/resolve/main/LTX25dist-echoVid-100T50-v2-DiT-Q5_K_M.gguf) |
| **2.5** | GGUF | `echoVid 100T50` | ![Q6_K][badge-Q6_K] | 17.75 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf/resolve/main/LTX25dist-echoVid-100T50-v2-DiT-Q6_K.gguf) |
| **2.5** | GGUF | `echoVid 100T50` | ![Q8_0][badge-Q8_0] | 22.73 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx25-echoVid-gguf/resolve/main/LTX25dist-echoVid-100T50-v2-DiT-Q8_0.gguf) |

</details>

<p id="finetune-pinkcherry" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ PinkCherry NSFW

Repo: [`SexGod1979/PinkCherry_NSFW_LTX23`](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23) — uncensored NSFW LTX-2.3 finetune family (NSFW content only — do not use for clean content). Pairs with the official LTX-2.3 distilled LoRA 384.

| Variant | Precision | Size | Download |
| :--- | :---: | :---: | :--- |
| v1.3 dev | ![bf16][badge-bf16] | 46.14 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.3/SexGod_PinkCherry_dev_bf16_LTX23_v1_3.safetensors) |
| v1.3 dev | ![fp8](https://img.shields.io/badge/fp8-17a2b8?style=flat-square) | 27.62 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.3/SexGod_PinkCherry_dev_fp8_plain_LTX23_v1_3.safetensors) |
| v1.5 dev | ![bf16][badge-bf16] | 46.14 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.5/SexGod_PinkCherry_dev_bf16_LTX23_v1_5.safetensors) |
| v1.5 dev | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 27.64 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.5/SexGod_PinkCherry_dev_int8_v1_5.safetensors) |
| v1.6 dev | ![bf16][badge-bf16] | 46.14 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.6/SexGod_PinkCherry_dev_bf16_LTX23_v16b.safetensors) |
| v1.6 dev | ![fp8](https://img.shields.io/badge/fp8-17a2b8?style=flat-square) | 27.62 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.6/SexGod_PinkCherry_dev_fp8scaled_LTX23_v16b.safetensors) |
| v1.6 dev | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 27.64 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.6/SexGod_PinkCherry_dev_int8_LTX23_v16b.safetensors) |
| v1.7-alpha dev | ![bf16][badge-bf16] | 46.14 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.7-alpha/PinkCherry_FineTune_bf16_v1_7-alpha.safetensors) |
| v1.7-alpha dev | ![fp8](https://img.shields.io/badge/fp8-17a2b8?style=flat-square) | 27.62 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.7-alpha/PinkCherry_FineTune_fp8scaled_v1_7-alpha.safetensors) |
| v1.7-alpha dev | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 27.64 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.7-alpha/PinkCherry_FineTune_int8_v1_7-alpha.safetensors) |
| v1.8 dev | ![bf16][badge-bf16] | 46.14 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.8/PinkCherry_FineTune_bf16_v1_8_LTX23.safetensors) |
| v1.8 dev | ![fp8](https://img.shields.io/badge/fp8-17a2b8?style=flat-square) | 27.62 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.8/PinkCherry_FineTune_fp8scaled_v1_8_LTX23.safetensors) |
| v1.8 dev | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 27.64 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.8/PinkCherry_FineTune_int8_v1_8_LTX23.safetensors) |

◦ **PinkCherry GGUF** — low-VRAM quants by SexGod1979

<details>
  <summary>v1.7-alpha / v1.8 GGUF</summary>

| Quant | Build | Size | Download |
| :--- | :---: | :---: | :--- |
| ![Q5_K_M][badge-Q5_K_M] | v1.7-alpha | 15.93 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.7-alpha/PinkCherry_FineTune_Q5_K_M_v1_7-alpha.gguf) |
| ![Q6_K][badge-Q6_K] | v1.7-alpha | 17.77 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.7-alpha/PinkCherry_FineTune_Q6_K_v1_7-alpha.gguf) |
| ![Q5_K_M][badge-Q5_K_M] | v1.8 | 15.93 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.8/PinkCherry_FineTune_Q5_K_M_v18_LTX23.gguf) |
| ![Q8_0][badge-Q8_0] | v1.8 | 22.76 GB | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.8/PinkCherry_FineTune_Q8_0_v1_8_LTX23.gguf) |

</details>

#### ❖ Elastic

Elastic is a TensorRT-engine distribution of a LoRA-integrated distilled FP8 T2V variant of LTX-2.3, packaged by [TheStageAI](https://huggingface.co/TheStageAI/Elastic-LTX-2.3) as `.qlip` shard files for H100 GPUs.

| Build | Name | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| distil + LoRA T2V | `Elastic — H100` | fp8 | ~19 GB (49 `.qlip` shards) | [![TheStageAI][gh-TheStageAI]](https://huggingface.co/TheStageAI/Elastic-LTX-2.3/tree/main/models/H100/ltx-2.3-22b-distilled-fp8-t2v_lora) |

<p id="finetune-chriscoletech-23" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ ChrisColeTech Uncensored Turbo (LTX-2.3)

Pre-merged **LTX-2.3 Uncensored Turbo** DiT by [ChrisColeTech](https://huggingface.co/ChrisColeTech) with three fine-tunes baked into the weights: 10Eros NSFW LoRA (1.0), DMD distilled LoRA (1.0, 4-step capable — 8 steps recommended), and the official LTXV ICLoRA Detailer (0.6). Modes: T2AV / I2AV / V2V / A2V / REF2VA; example workflows bundled in the repo. **v1.4** is the build documented in the card; the repo tree has since gained a **v1.5 fp8_scaled** DiT (21.12 GB) that the card does not describe yet.

| Ver | Build | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.3** | v1.4 fp8mixed | ![fp8][badge-fp8] | 29.16 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.3-uncensored-v1.4-FP8/resolve/main/split/diffusion_models/ltxv23_uncensored_v1.4_fp8mixed.safetensors) |
| **2.3** | v1.5 fp8_scaled | ![fp8][badge-fp8] | 21.12 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.3-uncensored-v1.4-FP8/resolve/main/split/diffusion_models/v1.5/ltxv23_uncensored_v1.5-fp8_scaled.safetensors) |
| **2.3** | v1.4 GGUF | ![Q4_K_M][badge-Q4_K_M] | 14.18 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.3-uncensored-v1.4-FP8/resolve/main/split/diffusion_models/ltxv23_uncensored_v1.4_Q4_K_M.gguf) |
| **2.3** | v1.4 GGUF | ![Q6_K][badge-Q6_K] | 17.76 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.3-uncensored-v1.4-FP8/resolve/main/split/diffusion_models/ltxv23_uncensored_v1.4_Q6_K.gguf) |
| **2.3** | v1.4 GGUF | ![Q8_0][badge-Q8_0] | 22.74 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.3-uncensored-v1.4-FP8/resolve/main/split/diffusion_models/ltxv23_uncensored_v1.4_Q8_0.gguf) |

◦ **Component splits** live in the same repo under `split/`: the uncensored **v1.4 projections** (`ltxv23_uncensored_v1.4_projections.safetensors`, 2.31 GB — required, goes in `text_encoders/`), an abliterated **Gemma-3-12b Q4_K_M** encoder with bi-projections (7.30 GB), the uncensored v1.4 audio / video VAEs, the older **v1.0** uncensored build, a stock **LTX-2.3 distilled fp8** under `v1.0/distilled_base/`, and LTX-2.3 spatial upscalers x2 1.0 / 1.1 — see the repo tree for the full list.

<details>
  <summary>v1.0 builds (older, also in this repo)</summary>

| Ver | Build | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.3** | v1.0 fp8 | ![fp8][badge-fp8] | 29.16 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.3-uncensored-v1.4-FP8/resolve/main/split/diffusion_models/v1.0/ltx-2.3-22b-uncensored-fp8.safetensors) |
| **2.3** | v1.0 int8 | ![int8tensormixed][badge-int8tensormixed] | 29.16 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.3-uncensored-v1.4-FP8/resolve/main/split/diffusion_models/v1.0/ltx-2.3-22b-uncensored-int8.safetensors) |
| **2.3** | v1.0 GGUF | ![Q4_K_M][badge-Q4_K_M] | 14.30 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.3-uncensored-v1.4-FP8/resolve/main/split/diffusion_models/v1.0/ltx-2.3-22b-uncensored-Q4_K_M.gguf) |
| **2.3** | v1.0 GGUF | ![Q6_K][badge-Q6_K] | 17.77 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.3-uncensored-v1.4-FP8/resolve/main/split/diffusion_models/v1.0/ltx-2.3-22b-uncensored-Q6_K.gguf) |
| **2.3** | v1.0 GGUF | ![Q8_0][badge-Q8_0] | 22.76 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.3-uncensored-v1.4-FP8/resolve/main/split/diffusion_models/v1.0/ltx-2.3-22b-uncensored-Q8_0.gguf) |
| **2.3** | v1.0 distilled fp8 (stock base) | ![fp8][badge-fp8] | 29.53 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.3-uncensored-v1.4-FP8/resolve/main/split/diffusion_models/v1.0/distilled_base/ltx-2.3-22b-distilled-fp8.safetensors) |

</details>

<p id="finetune-chriscoletech-25" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ ChrisColeTech Uncensored Turbo v1.1 (LTX-2.5)

Pre-merged **LTX-2.5 Extreme Uncensored Turbo v1.1** DiT by [ChrisColeTech](https://huggingface.co/ChrisColeTech) — *"Eros10 NSFW & 4-step LoRA baked-in"*. **Five** fine-tunes are baked into the weights: the **10Eros NSFW** LoRA (0.7), the **DMD distilled** LoRA (1.0 — 4 steps work, 8 recommended), the official **LTXV IC-LoRA** (0.7), the **IC-LoRA Detailer** (0.45, for V2V control on top of T2V/I2V) and an **Img2Vid adapter** LoRA (0.45). Base is `Lightricks/LTX-2.5`; modes T2V / I2V / V2V / A2V / REF2VA.

Because the IC-LoRA is baked in, prompts can use the `[VISUAL]` / `[SPEECH]` / `[SOUNDS]` template blocks for precise control of picture, dialogue and ambience. Recommended settings: 1280×720, 124 frames @ 24 fps, **8 steps** (16 max), guidance 1.0.

> ⚠️ The repo was previously published as `ChrisColeTech/LTX-2.5-turbo-GGUF`; the old URL now redirects here. The **card's own component links are broken** — it names `ltx25_uncensored_v1.1_audio_vae` / `..._video_vae`, but the files on disk are `ltx25_uncensored_audio_vae` / `ltx25_uncensored_video_vae` (no `v1.1` infix).

| Ver | Build | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.5** | v1.1 fp8 | ![fp8][badge-fp8] | 21.02 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.5-uncensored-v1.1-FP8/resolve/main/split/diffusion_models/ltx25_uncensored_v1.1-fp8.safetensors) |
| **2.5** | v1.1 fp8 (scaled) | ![fp8][badge-fp8] | 21.47 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.5-uncensored-v1.1-FP8/resolve/main/split/diffusion_models/ltx25_uncensored_v1.1-fp8_scaled.safetensors) |
| **2.5** | v1.1 int8 | ![int8tensormixed][badge-int8tensormixed] | 21.47 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.5-uncensored-v1.1-FP8/resolve/main/split/diffusion_models/ltx25_uncensored_v1.1-int8.safetensors) |
| **2.5** | v1.1 GGUF | ![Q4_K_M][badge-Q4_K_M] | 14.18 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.5-uncensored-v1.1-FP8/resolve/main/split/diffusion_models/ltx25_uncensored_v1.1-Q4_K_M.gguf) |
| **2.5** | v1.1 GGUF | ![Q6_K][badge-Q6_K] | 17.76 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.5-uncensored-v1.1-FP8/resolve/main/split/diffusion_models/ltx25_uncensored_v1.1-Q6_K.gguf) |
| **2.5** | v1.1 GGUF | ![Q8_0][badge-Q8_0] | 22.33 GB | [![ChrisColeTech][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.5-uncensored-v1.1-FP8/resolve/main/split/diffusion_models/ltx25_uncensored_v1.1-Q8_0.gguf) |

◦ **Precision, verified from the safetensors headers** — `fp8` = 4,349 tensors (BF16 × 2,577 + F8_E4M3 × 1,772, unscaled); `fp8_scaled` = 5,789 tensors (BF16 × 2,909 + F8_E4M3 × 1,440 + F32 × 1,440 scales); `int8` = 5,789 tensors (BF16 × 2,909 + **I8** × 1,440 + F32 × 1,440), metadata `quantization: int8_tensorwise` — the weights are stored as `float8_e4m3fn` with per-layer scales and full-precision matrix multiplies. All three are `AVTransformer3DModel`, `model_version 2.5.0`, `gemma4-12b-ltx-v1`.

◦ **Component splits** in the same repo under `split/`: the **uncensored Gemma-4-12b** text encoder with the LTX projections already baked in (`gemma4_12b_ltx25_uncensored-int8.safetensors`, 13.16 GB — see [Gemma-4-12b](#enc-gemma4)), its GGUF variants, the **uncensored video / audio VAEs** (byte-identical to the official `Lightricks/LTX-2.5` VAEs) and the LTX-2.5 spatial / temporal latent upscalers x2.

<p id="finetune-redgraft" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ REDGraft (NSFW)

Uncensored NSFW **LTX-2.5** checkpoint by [EllaPriest45](https://huggingface.co/EllaPriest45) ("REDGraft"), shipped as a single INT8 full checkpoint together with a bundled two-stage i2V workflow JSON (ManualSigmas ×2 + LoRA loader).

| Ver | Build | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.5** | REDGraft NSFW (full ckpt) | ![int8tensormixed][badge-int8tensormixed] | 17.03 GB | [![EllaPriest45][gh-EllaPriest45]](https://huggingface.co/EllaPriest45/LTX2.5_checkpoints/resolve/main/REDGraft%20%28NSFW%29%20INT8%20-%20LTX2.5.safetensors) |

◦ Bundled workflow: [`REDGraft (NSFW) INT8 - LTX2.5.json`](https://huggingface.co/EllaPriest45/LTX2.5_checkpoints/resolve/main/REDGraft%20%28NSFW%29%20INT8%20-%20LTX2.5.json).

<p id="finetune-colinb83-nsfw" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ colinb83 NSFW (LTX-2.5 full FT)

A **full bf16 fine-tune of the LTX-2.5 22B DiT** on a 54,702-clip NSFW corpus (1280×704, 10 s + 5 s clips) by [colinb83](https://huggingface.co/colinb83) — the final checkpoint of the completed 7,000-step run. All **48 transformer blocks** were trained (18.56B params, 4,032 tensors) with a streaming dense full fine-tune using stochastic-BF16 Adafactor; connectors and non-block tensors are the original base weights. Single RTX PRO 6000 Blackwell with ring offload (8 blocks swapped / 2-block double buffer), ~38 h total.

| Ver | Build | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.5** | NSFW full FT (step 7000) | ![bf16][badge-bf16] | 42.01 GB | [![colinb83][gh-colinb83]](https://huggingface.co/colinb83/ltx-2.5-nsfw-step7000/resolve/main/ltx-2.5-nsfw-step7000.safetensors) |
| **2.5** | NSFW full FT (step 4500 test merge) | ![bf16][badge-bf16] | 42.01 GB | [![colinb83][gh-colinb83]](https://huggingface.co/colinb83/KimCherry4500test/resolve/main/KimCherry4500test.safetensors) |

◦ **Base / requirements:** LTX-2.5 22B dev (`AVTransformer3DModel`, `model_version: 2.5.0`). The card declares an **abliterated Gemma 4 12B text encoder (`gemma4-12b-ltx-v1`)** — use that encoder plus the standard LTX-2.5 video/audio VAEs. Load with **UNETLoader** as a standard LTX-2.5 checkpoint in any ComfyUI workflow.

◦ **Training recipe:** 2,000 steps @ 1e-5 then 5,000 steps @ 3e-6 (constant per phase), batch 1, gradient checkpointing on. Trained at 1280×704 × 97 frames (~10 s); captions are long-form, camera-first, present-tense descriptions.

◦ ⚠️ **Distill LoRAs do not transfer cleanly.** Distillation LoRAs made for the unmodified dev model (e.g. `ltx-2.5-22b-distilled-lora-450`) apply a weight delta ~**44%** the magnitude of this fine-tune and are calibrated against the original base — use them at reduced strength or retrain one against this checkpoint.

◦ **No model card in the repo itself** (the tree holds only the weights file + `.gitattributes`); the documentation above comes from the author's sibling repo [`colinb83/ltx-2.5-nsfw`](https://huggingface.co/colinb83/ltx-2.5-nsfw), which ships the same final checkpoint plus an earlier `dense_weights_step_00250.safetensors` (28.24 GB) snapshot.

◦ **Step-4500 test merge** — an intermediate snapshot of the same run, published as a separate **public** repo [`colinb83/KimCherry4500test`](https://huggingface.co/colinb83/KimCherry4500test) (commit title *“LTX-2.5 22B NSFW full fine-tune, step 4500 test merge”*). Its header matches the final checkpoint exactly — 4,349 tensors, the same `model.diffusion_model.*` key set over 48 blocks, `AVTransformer3DModel` — but keeps **146 F32 scale-shift tables** (`scale_shift_table`, `audio_scale_shift_table`, `audio_prompt_scale_shift_table`, `scale_shift_table_a2v_ca_audio`) where the step-7000 file has only 2, i.e. it is the pre-BF16-cast merge state of the same training run rather than a differently-trained model. The repo has no model card either — the single file is `KimCherry4500test.safetensors`.

◦ **License:** subject to the **LTX-2.x Community License Agreement** (full text embedded in the safetensors metadata); derivatives of LTX-2.x must be distributed under that agreement. Content is NSFW/adult — the repo carries the `not-for-all-audiences` tag.

<p id="finetune-spatialav2av" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ SpatialAV2AV (BingoG)

Publicly-released audio→audio-video training checkpoints from [BingoG/LTX-2-SpatialAV2AV-Checkpoints](https://huggingface.co/BingoG/LTX-2-SpatialAV2AV-Checkpoints) for spatial-audio conditioned video generation. Two curriculum layouts (`E4` Core Dual + Dynamic; `E6` reserved for Full) at 480p cap, 113 frames at 25 fps.

| Curriculum | Step | Size | Download |
| :--- | :---: | :---: | :---: |
| E4 Core (Dual + Dynamic) | 400  | 37.98 GB | [![BingoG][gh-BingoG]](https://huggingface.co/BingoG/LTX-2-SpatialAV2AV-Checkpoints/resolve/main/E4/step_00400/model_weights_step_00400.safetensors) |
| E4 Core (Dual + Dynamic) | 1000 | 37.98 GB | [![BingoG][gh-BingoG]](https://huggingface.co/BingoG/LTX-2-SpatialAV2AV-Checkpoints/resolve/main/E4/step_01000/model_weights_step_01000.safetensors) |
| E6 Full                  | 1000 | 37.98 GB | [![BingoG][gh-BingoG]](https://huggingface.co/BingoG/LTX-2-SpatialAV2AV-Checkpoints/resolve/main/E6/step_01000/model_weights_step_01000.safetensors) |

*Note: these are intermediate training checkpoints, not inference-ready models — useful for fine-tuning experiments and reproducibility only.*

<p id="finetune-onestep-refiner" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ One-Step Refiner (Owen777)

One-step **LTX-2.5** video refiner by [Owen777](https://huggingface.co/Owen777) — a DMD/GAN-style one-step refinement model (EMA step 835) that sharpens/refines generated video in a single pass. **Access is gated** — request access on the repo before downloading.

| Ver | Build | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.5** | one-step refiner (EMA step 835) | ![bf16][badge-bf16] | 26.25 GB | [![Owen777][gh-Owen777]](https://huggingface.co/Owen777/LTX2.5-One-Step-Refiner-Step835/resolve/main/step_00000835_ema_bf16.safetensors) |

◦ Reinforcement-learning LoRA also in repo: [`rl_lora/step_000400.pt`](https://huggingface.co/Owen777/LTX2.5-One-Step-Refiner-Step835/resolve/main/rl_lora/step_000400.pt) (~0.81 GB).

#### ❖ SoL-Refiner — one-step 1080p/2K upscaler (szwagros, int8 ConvRot)

Generic one-step refiner from NVlabs' [SoL-Refiner](https://nvlabs.github.io/Sana/Sol-Refiner/) project (SANA / SANA-Video): a cheap low-res draft (SANA-Video, WAN, MiniMax-H3, …) is encoded, **2x latent-upscaled with AdaIN**, re-noised and denoised in a **single** transformer forward, turning the draft into 1080p/2K output. Repackaged by [szwagros](https://huggingface.co/szwagros) from the `Efficient-Large-Model` originals into the **image-server `ltx_core` layout** (`diffusion_models/` + `text_encoders/` + `vae/` + `latent_upscale_models/`) — the transformer and text encoder are int8 ConvRot and expect the `image_server_kernels.int8_linear` backend, so these are **not** drop-in ComfyUI checkpoints.

**LTX-2.3 One-Step** — [szwagros/SoL-Refiner-LTX-2.3-One-Step-int8-convrot](https://huggingface.co/szwagros/SoL-Refiner-LTX-2.3-One-Step-int8-convrot) · **41.93 GB** total · re-noised to sigma 0.725

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `sol-refiner-ltx-2.3-one-step-transformer-comfy-int8-convrot` (DiT) | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 23.51 GB | [![][gh-szwagros]](https://huggingface.co/szwagros/SoL-Refiner-LTX-2.3-One-Step-int8-convrot/resolve/main/diffusion_models/sol-refiner-ltx-2.3-one-step-transformer-comfy-int8-convrot.safetensors) |
| `gemma3-12b-with-proj-…-comfy-int8-convrot` (text encoder) | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 15.97 GB | [![][gh-szwagros]](https://huggingface.co/szwagros/SoL-Refiner-LTX-2.3-One-Step-int8-convrot/resolve/main/text_encoders/gemma3-12b-with-proj-sol-refiner-ltx-2.3-one-step-comfy-int8-convrot.safetensors) |
| `ltx-2.3-22b_vae` (video VAE) | ![bf16][badge-bf16] | 1.45 GB | [![][gh-szwagros]](https://huggingface.co/szwagros/SoL-Refiner-LTX-2.3-One-Step-int8-convrot/resolve/main/vae/ltx-2.3-22b_vae.safetensors) |
| `ltx-2.3-spatial-upscaler-x2-1.1` (x2 latent upsampler) | ![bf16][badge-bf16] | 1.00 GB | [![][gh-szwagros]](https://huggingface.co/szwagros/SoL-Refiner-LTX-2.3-One-Step-int8-convrot/resolve/main/latent_upscale_models/ltx-2.3-spatial-upscaler-x2-1.1.safetensors) |

⚠️ Always condition with **`frame_rate=16`**, whatever the input fps (encode the output at the real fps) — the model was trained on 16 fps drafts and a 24 fps value mis-scales the temporal RoPE and ghosts moving objects. Uses the **v1.1** x2 upsampler, not v1.0.

**LTX-2.5 for MiniMax-H3** — [szwagros/SoL-Refiner-LTX-2.5-H3-int8-convrot](https://huggingface.co/szwagros/SoL-Refiner-LTX-2.5-H3-int8-convrot) · **41.35 GB** total · re-noised to sigma 0.909375

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `sol-refiner-ltx-2.5-h3-transformer-comfy-int8-convrot` (DiT) | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 23.51 GB | [![][gh-szwagros]](https://huggingface.co/szwagros/SoL-Refiner-LTX-2.5-H3-int8-convrot/resolve/main/diffusion_models/sol-refiner-ltx-2.5-h3-transformer-comfy-int8-convrot.safetensors) |
| `gemma4-12b-with-proj-…-comfy-int8-convrot` (text encoder) | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 15.37 GB | [![][gh-szwagros]](https://huggingface.co/szwagros/SoL-Refiner-LTX-2.5-H3-int8-convrot/resolve/main/text_encoders/gemma4-12b-with-proj-sol-refiner-ltx-2.5-h3-comfy-int8-convrot.safetensors) |
| `sol-refiner-ltx-2.5-h3-video-vae-bf16` (VAE + diffusion decoder) | ![bf16][badge-bf16] | 1.47 GB | [![][gh-szwagros]](https://huggingface.co/szwagros/SoL-Refiner-LTX-2.5-H3-int8-convrot/resolve/main/vae/sol-refiner-ltx-2.5-h3-video-vae-bf16.safetensors) |
| `ltx-2.5-latent-spatial-upscaler-x2-bf16-1.0` (x2 latent upsampler) | ![bf16][badge-bf16] | 1.00 GB | [![][gh-szwagros]](https://huggingface.co/szwagros/SoL-Refiner-LTX-2.5-H3-int8-convrot/resolve/main/latent_upscale_models/ltx-2.5-latent-spatial-upscaler-x2-bf16-1.0.safetensors) |

◦ Conditioning `frame_rate` = the input fps (H3 drafts are 24 fps). One step, no CFG. **Video output only — no audio.** The text encoder is the refiner's shipped Gemma 4, i.e. the **pre-2026-08-17** Lightricks encoder rather than the current one.

◦ Both are finetunes of LTX-2.x, so the **LTX-2.x Community License** (Lightricks) applies — check it before commercial use. Source repos: [2.3 One-Step](https://huggingface.co/Efficient-Large-Model/SoL-Refiner-LTX-2.3-One-Step) · [2.5 for MiniMax-H3](https://huggingface.co/Efficient-Large-Model/SoL-Refiner-LTX-2.5-for-MiniMax-H3).

<p id="finetune-solarwm" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ SolarWM (World Model)

Research **LTX-2.5 world model** by [junchaoh-cs](https://huggingface.co/junchaoh-cs) (arXiv:[2609.02886](https://arxiv.org/abs/2609.02886)) — a long-horizon, camera-controllable video world model finetuned from LTX-2.5 22B. The repo re-ships the LTX-2.5 22B base (dev transformer + gemma4-12b text encoder + VAE) plus a finetuned stage, `SolarWM-ltx-22B-bid-stage0p5-153f` (EMA weights, `ema/model.safetensors`). **Access is gated** — request access before downloading; exact artifact formats are unconfirmed (gated).

| Ver | Build | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.5** | SolarWM bid-stage0p5-153f (finetuned stage) | — | 3.93 GB | [![junchaoh-cs][gh-junchaoh-cs]](https://huggingface.co/junchaoh-cs/SolarWM-LTX-22B/resolve/main/SolarWM-ltx-22B-bid-stage0p5-153f/ema/model.safetensors) |

◦ Base LTX-2.5 22B (dev transformer + gemma4-12b encoder + VAE) also in repo. Paper: [arXiv:2609.02886](https://arxiv.org/abs/2609.02886).

<p id="finetune-stubelius" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ Stubelius Remix (Stuubs)

**LTX-2.5** merged finetune by [Stuubs](https://huggingface.co/Stuubs) (12 likes) — the **distilled LoRA baked in**, plus (from v1) **OmniNFT** RL-finetune merged at its trained strength. Mainly aimed at NSFW but works SFW (name clothing explicitly in SFW prompts or you may get unwanted nudity). Ships three v1 builds plus two beta builds; **use v1**.

| Ver | Build | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.5** | `v1` (recommended, ComfyUI int8) | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 21.50 GB | [![Stuubs][gh-Stuubs]](https://huggingface.co/Stuubs/Stubelius_Remix_Ltx2.5/resolve/main/ltx2.5-Stubelius_remix_v1_int8_convrot.safetensors) |
| **2.5** | `v1` (merging / own conversions) | ![bf16][badge-bf16] | 42.01 GB | [![Stuubs][gh-Stuubs]](https://huggingface.co/Stuubs/Stubelius_Remix_Ltx2.5/resolve/main/ltx2.5-Stubelius_remix_v1_bf16.safetensors) |
| **2.5** | `v1` NVFP4 (RTX 50-series only, **experimental**) | ![nvfp4][badge-nvfp4] | 14.40 GB | [![Stuubs][gh-Stuubs]](https://huggingface.co/Stuubs/Stubelius_Remix_Ltx2.5/resolve/main/ltx2.5-Stubelius_remix_v1_nvfp4.safetensors) |
| **2.5** | `beta2` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 21.50 GB | [![Stuubs][gh-Stuubs]](https://huggingface.co/Stuubs/Stubelius_Remix_Ltx2.5/resolve/main/ltx2.5-Stubelius_remix_beta2_int8_convrot.safetensors) |
| **2.5** | `beta2` | ![bf16][badge-bf16] | 42.01 GB | [![Stuubs][gh-Stuubs]](https://huggingface.co/Stuubs/Stubelius_Remix_Ltx2.5/resolve/main/ltx2.5-Stubelius_remix_beta2_bf16.safetensors) |
| **2.5** | `beta1` | ![bf16][badge-bf16] | 42.01 GB | [![Stuubs][gh-Stuubs]](https://huggingface.co/Stuubs/Stubelius_Remix_Ltx2.5/resolve/main/ltx2.5-Stubelius_remix_beta1.safetensors) |

◦ **Run it:** drop the int8 file in `ComfyUI/models/diffusion_models`, load with **Load Diffusion Model** (or pick it in the Models node of *Stubelius Ultimate LTX 2.5*). **CFG 1, 8 steps** (+3–4 if you run an upscale pass). Do **not** add a distilled LoRA or OmniNFT on top — both are already baked in. Needs `gemma4-12b-with-proj-ltx-2.5-comfy-int8-convrot.safetensors` (Lightricks re-uploaded it in mid-August — re-download if yours is older) plus `ltx-2.5-video-vae-bf16` and `ltx-2.5-audio-vae-bf16`.

◦ **v1 vs beta2, per the author:** +55% sharper fine detail (faces, hair, fabric, backgrounds), +15% more motion, same remix / prompt-following / loudness, dialogue still verbatim. Blind AI-judged A/B of full-res frames: OmniNFT at v1's strength won **29–9** with 10 ties. A few scenes come out less saturated on average. VBVR was tested and **rejected** — it cost motion without improving prompt following.

◦ **NVFP4 is experimental:** transformer blocks 0–41 in NVFP4, last 6 blocks + text connectors in int8 (Lightricks' own layer choice). Fast only on RTX 50-series (Blackwell) with ComfyUI ≥ 0.32 and PyTorch built for CUDA 13; older cards run it but slower than int8. Renders haven't been fully compared against int8 yet.

◦ The int8 build needs a recent enough ComfyUI to load Comfy-Org's int8 LTX-2.5 files. LTX-2.5 LoRAs load on it the same way as on stock LTX-2.5. Credits: Lightricks (LTX-2.5 + distilled LoRA), FusionCow / Sulp.

<p id="finetune-ellapriest45" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ EllaPriest45 (model mirror)

> **Note:** the EllaPriest45 LTX collection is **split across sub-repos**, not one monorepo. Older revisions of this list linked a single `EllaPriest45/LTX2.5_checkpoints`; the same author also mirrors LTX weights under 14 sibling repos.

| Sub-repo | Contents | Size |
| :--- | :--- | ---: |
| [`LTX2.5_checkpoints`](https://huggingface.co/EllaPriest45/LTX2.5_checkpoints) | Full checkpoints — REDGraft NSFW int8, plus Joy-LTX / Q3_K_M GGUFs | 40.6 GB |
| [`LTX2.5_base`](https://huggingface.co/EllaPriest45/LTX2.5_base) | Base runtime — turbo distill LoRAs (r450/r256/r128), VAEs, upscalers, MSR LoRA, Q4_K_M + Gemma-4 Q5_K_M GGUFs, ComfyUI node zips | 45.7 GB |
| [`LTX2.5_actions`](https://huggingface.co/EllaPriest45/LTX2.5_actions) | Face-swap (BFS r128/r64), EditAnything v2.0, Alpha Gen, BTS Movie Set, NSFW action LoRAs + bundled workflow JSONs | 7.9 GB |
| [`LTX2.5_styles`](https://huggingface.co/EllaPriest45/LTX2.5_styles) | **3D Animation Style** (0.674 GB) — the only weight left in this sub-repo | 0.7 GB |
| [`LTX2.3_checkpoints`](https://huggingface.co/EllaPriest45/LTX2.3_checkpoints) | 10Eros v1.4 Bob int8-ConvRot, PinkCherry v1.8 Q5_KM, DaSiWa DragonLeap Q4_K_M, JoyAI-Echo surgical Q5, INT4-Quality dev, GGUF Companion, plus two `fro99-AVGRank104` averaged LoRA merges (listed below) | 122.3 GB |
| [`LTX2.3_base`](https://huggingface.co/EllaPriest45/LTX2.3_base) | LTX-2.3 dev int8-ConvRot, Sulphur dev fp8mixed, Gemma-3 encoder variants, connectors, VAEs, upscalers, ID/OmniNFT/distill LoRAs | 187.9 GB |
| [`LTX2.3_Actions`](https://huggingface.co/EllaPriest45/LTX2.3_Actions) | NSFW action / motion LoRAs, EditAnything v1.1, Best-FaceID, OmniCine | 154.9 GB |
| [`LTX2.3_Characters`](https://huggingface.co/EllaPriest45/LTX2.3_Characters) | Per-celebrity / per-character likeness LoRAs (394 files) | 139.3 GB |
| [`LTX2.3_Styles`](https://huggingface.co/EllaPriest45/LTX2.3_Styles) | Visual-style LoRAs — anime, claymation, cyberpunk, post-apocalyptic, Dispatch, GalaxyAce, furry | 25.7 GB |
| [`LTX2.3_Dramabox`](https://huggingface.co/EllaPriest45/LTX2.3_Dramabox) | DramaBox audio DiT + audio components (unsplit pair) | 8.5 GB |
| [`LTX2.3_workflows`](https://huggingface.co/EllaPriest45/LTX2.3_workflows) | 155 ComfyUI workflow JSONs | 0.7 GB |
| [`LTX2.3`](https://huggingface.co/EllaPriest45/LTX2.3) | LTX-2.3 LoRAs — lipdub IC-LoRA, NSFW Helper v2.0, NSFW Posing Nude, GalaxyAce, Crisp / Soft Enhance, VBVR video-reasoning, Boudoir, Camera Controls, Stylized PBR Animation, Mystic XXX, Amateur Hour r16, epic_cumshots + helper `.py` scripts and workflow JSONs | 12.0 GB |
| [`LTX2_oldstuff`](https://huggingface.co/EllaPriest45/LTX2_oldstuff) | Legacy **LTX-2 (v2.0)** LoRAs — 37 weights: NSFW action / pose (Tit-Daddy v2.0, Oral Suite, POV NSFW v3.0, Doggy Style, Sexy Move, Best Breasts v2.0, Pillow Humping, …), face swap (BFS v1 focus head), character (Aerith, Jessica Rabbit, Artemis, Gollum), styles (Dispatch v3, Manga, Anime Flat, GalaxyAce) and IC-LoRA Detailer (+ 3 PDF cards) | 29.9 GB |
| [`dramabox-dit-int8`](https://huggingface.co/EllaPriest45/dramabox-dit-int8) | DramaBox TTS 3.3B DiT — selective INT8 weight-only quant (562 layers) + `config.json` / loader scripts | 3.6 GB |

The `LTX2.5_styles` and `LTX2.5_actions` LoRAs are listed individually under [`▣ Styles`](#lora-styles) and [`▣ Special`](#lora-special); the GGUFs under [GGUF Quantized Models](#gguf); REDGraft under [`REDGraft (NSFW)`](#finetune-redgraft).

**Selected non-LoRA weights worth calling out** (all links verified; most are re-packs of models listed from their primary sources elsewhere on this page):

| Weights | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `LTX 2.3 dev INT8 ConvRot` (standalone, not in LTX-2.3/Comfy) | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 23.51 GB | [![EllaPriest45][gh-EllaPriest45]](https://huggingface.co/EllaPriest45/LTX2.3_base/resolve/main/LTX%202.3%20dev%20INT8%20ConvRot%20-%20LTX2.3.safetensors) |
| `Diffusion Models - Sulphur_dev_model_fp8mixed` | ![fp8][badge-fp8] | 25.03 GB | [![EllaPriest45][gh-EllaPriest45]](https://huggingface.co/EllaPriest45/LTX2.3_base/resolve/main/Diffusion%20Models%20-%20Sulphur_dev_model_fp8mixed.safetensors) |
| `LTX 2.3 INT8 Dev Transformer INT4 Quality` | ![int4][badge-int4] | 18.98 GB | [![EllaPriest45][gh-EllaPriest45]](https://huggingface.co/EllaPriest45/LTX2.3_checkpoints/resolve/main/LTX%202.3%20INT8%20Dev%20Transformer%20INT4%20Quality%20-%20LTX2.3.safetensors) |
| `LTX-2.3 GGUF Companion` (transformer-only split for GGUF loading) | ![bf16][badge-bf16] | 9.02 GB | [![EllaPriest45][gh-EllaPriest45]](https://huggingface.co/EllaPriest45/LTX2.3_checkpoints/resolve/main/LTX-2.3%20GGUF%20Companion%20-%20LTX2.3.safetensors) |
| `DramaBox audio DiT v1` | ![bf16][badge-bf16] | 6.58 GB | [![EllaPriest45][gh-EllaPriest45]](https://huggingface.co/EllaPriest45/LTX2.3_Dramabox/resolve/main/models_dramabox-dit-v1.safetensors) |
| `DramaBox audio DiT v1 — INT8 selective` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 3.62 GB | [![EllaPriest45][gh-EllaPriest45]](https://huggingface.co/EllaPriest45/dramabox-dit-int8/resolve/main/dramabox-dit-int8-selective.safetensors) |
| `DramaBox audio components` (vocoder / Mel-band / TAE bundle) | ![bf16][badge-bf16] | 1.94 GB | [![EllaPriest45][gh-EllaPriest45]](https://huggingface.co/EllaPriest45/LTX2.3_Dramabox/resolve/main/dramabox-audio-components.safetensors) |

◦ **Not all mirrors add anything.** The `10eros v1.4 Q6_K`, `DaSiWa DragonLeap v4.0 Q4KM`, `SexGod PinkCherry v1.8 Q5_KM` and `JoyAI-Echo × LTX-2.3 Surgical Merge Q5` GGUFs are re-packs of quants already listed from SexGod1979 / DaSiWa / joeygambino / vantagewithai — linked from those sections. `LTX2.3_base`'s `Sulphur_dev-Q3_K_M.gguf` and `LTX-2.3-22b-distilled-Q4_K_M.gguf` are likewise re-packs of quants already listed (Abiray / unsloth), so they are not duplicated here.

◦ **Re-verified 2026-10-13:** every sub-repo above has a **single commit** (all dated 2026-10-08) — the file counts and totals in this table are unchanged, so nothing new has landed since the audit. The `LTX2.5_actions` bullet under [`▣ Special`](#lora-special) names its LoRAs individually. **2026-10-27:** the three sub-repos added above (`LTX2.3`, `LTX2_oldstuff`, `dramabox-dit-int8`) were previously uncatalogued; their file counts and totals above come from the live tree API.

◦ `LTX2.5_base` also bundles the **ComfyUI node zips** it expects (`ComfyUI-JoyLTX25`, `ComfyUI-KJNodes`, `ComfyUI-LTX2.5-MSR`, `ComfyUI-Sage-EasyInstall`) — the repo is usable as a one-stop 2.5 drop folder.

◦ **Not LTX assets.** Three files inside `LTX2.3_base` are **not** LTX weights and therefore do not belong in the component tables: `Diffusion models - MelBandRoformer_fp32.safetensors` (0.91 GB, also present byte-for-byte as `LTX2.3 MelBandRoformer FP32 - LTX2.3.safetensors`) is a generic **Mel-band RoFormer audio separator** (684 tensors: `band_split` / `layers` / `mask_estimators`, all F32); `Model Upscaler nmkdSiaxCX_200k - LTX2.3.safetensors` (0.07 GB) is a generic **ESRGAN / RRDB pixel upscaler** (702 tensors, `model.0…8`, all F32); and `Text encoder - Qwen3.5-sulphur_prompt_enhancer-Q8_0.gguf` (9.53 GB) is the **Sulphur-2 prompt-enhancer LLM**, not an LTX text encoder — it is a re-pack of the official `prompt_enhancer/sulphur_prompt_enhancer_model-q8_0.gguf` (listed above).

◦ **The “Image Upscaler” is a LoRA.** `LTX Image Upscaler - LTX2.3 - 4psc4l1fy,…` (0.81 GB) is — despite the filename — an **LTX-2.3 LoRA**, not an upscaler model: the header holds 768 BF16 tensors, `diffusion_model.transformer_blocks.0…47` with `lora_A` / `lora_B` pairs, and the metadata reads `modelspec.architecture: LTX2/lora`, `ss_network_dim: 128`, `ss_network_alpha: 128`, `ss_ltx_version: 2.3`, base `ltx-2.3-22b-dev.safetensors`. It is listed under [LoRA → Special & Enhancers](#lora-special).
