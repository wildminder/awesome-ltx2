# Awesome LTX-2

A curated list of models, text encoders, and tools for the LTX-2 video generation suite.

![ltx-logo](https://github.com/user-attachments/assets/ee73cbc3-648b-47fa-9346-c4299919a060)


<div align="center">

[![Telegram][telegram-shield]][telegram-url]
[![X][x-shield]][x-url]

</div>

<details>
<summary><b>Table of Contents</b></summary>

* [Apps & Tools](#apps)
* [Models](#models)
  * [Checkpoints](#checkpoints)
    * [silveroxides Quantizations (mxfp8)](#ckpt-silveroxides)
    * [Distilled LoRA](#ckpt-distilled-lora)
    * [TenStrip Distilled LoRA Experiments](#ckpt-tenstrip-distilled-lora)
    * [Spatial Upscaler](#ckpt-spatial-upscaler)
    * [Temporal Upscaler](#ckpt-temporal-upscaler)
  * [Merges](#merges)
  * [Finetunes](#finetunes)
    * [DaSiWa](#finetune-dasiwa)
    * [10Eros](#finetune-10eros)
    * [Sulphur-2-base](#finetune-sulphur)
    * [PinkCherry NSFW](#finetune-pinkcherry)
  * [GGUF Quantized Models](#gguf)
* [Text Encoders](#text-encoder)
  * [Comfy-Org Optimized Encoders](#text-encoder)
  * [Gemma-3-12b Abliterated](#enc-abliterated)
  * [Gemma-3-12b IT Heretic](#enc-heretic)
* [Separated Components](#split)
  * [Diffusion Models (Transformer Only)](#split)
  * [VAE (Video & Audio)](#components-vae)
  * [Embedding Connectors & Text Projection](#components-embed)
* [LoRA](#lora)
  * [Enchancer, special](#lora)
  * [Styles](#lora-styles)
  * [Special](#lora-special)
  * [ID-LoRA (Identity-Driven In-Context LoRA)](#lora-id-lora)
* [ComfyUI Nodes](#nodes)
  * [Custom Node Collections](#nodes)
* [LoRA Training](#training)
  * [Primary Local Training Tools](#training)
  * [Cloud Training Platforms](#training-cloud)
  * [Essential Dataset & Captioning Tools](#training-dataset)
  * [Training Requirements Summary](#training-requirements)
* [Workflow & Technical Notes](#wf)
  * [RuneXX](#wf)
  * [Lightricks](#wf-lightricks)
  * [vrgamedevgirl84](#wf-vrgamedevgirl84)
  * [ComfyUI](#wf-comfyui)

</details>

<a id="intro"></a>

## Intro

* [LTX official Blog](https://ltx.io/blog)
* ComfyUI official [blogpost](https://blog.comfy.org/p/ltx-2-open-source-audio-video-ai)
* [Prompting Guide for LTX-2](https://ltx.io/model/model-blog/prompting-guide-for-ltx-2)
* [LTX-2 in ComfyUI Chattable KB](https://notebooklm.google.com/notebook/4f07f98c-75b6-4278-bde1-906f9899b60c)

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


<a id="models"></a>

## ▓ Models

LTX-2 models are available in various formats including full weights, transformers-only, and GGUF quantizations for efficient inference.

<a id="checkpoints"></a>

### ▣ Checkpoints

* **[Lightricks/LTX-2](https://huggingface.co/Lightricks/LTX-2)** - Official repository.
* **[Lightricks/LTX-2.3](https://huggingface.co/Lightricks/LTX-2.3)** - Official repository (latest version).
* **[Drbaph](https://huggingface.co/drbaph/LTX-2.3-FP8)** - Quantization

| Ver | Name | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.3** | `dev` | ![bf16][badge-bf16] | 46.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-22b-dev.safetensors) |
| **2.3** | `dev` | ![fp8][badge-fp8] | 29.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3-fp8/resolve/main/ltx-2.3-22b-dev-fp8.safetensors) |
| **2.3** | `dev` | ![fp8][badge-fp8] | 29.9 GB | [![][gh-drbaph]](https://huggingface.co/drbaph/LTX-2.3-FP8/resolve/main/ltx-2.3-22b-dev-fp8.safetensors) |
| **2.3** | `dev` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 29.1 GB | [![][gh-Winnougan]](https://huggingface.co/Winnougan/LTX-2.3-Dev-Int8/resolve/main/ltx-2.3-22b-dev_INT8.safetensors) |
| **2.3** | `dev` | ![nvfp4][badge-nvfp4] | 21.7 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3-nvfp4/resolve/main/ltx-2.3-22b-dev-nvfp4.safetensors) |
| **2.3** | `dev` | ![fp8][badge-fp8] | 29.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3-fp8/resolve/main/ltx-2.3-22b-dev-fp8.safetensors) |
| **2.3** | `distilled` | ![bf16][badge-bf16] | 46.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-22b-distilled.safetensors) |
| **2.3** | `distilled` | ![fp8][badge-fp8] | 29.5 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3-fp8/resolve/main/ltx-2.3-22b-distilled-fp8.safetensors) |
| **2.3** | `distilled` | ![fp8][badge-fp8] | 29.9 GB | [![][gh-drbaph]](https://huggingface.co/drbaph/LTX-2.3-FP8/resolve/main/ltx-2.3-22b-distilled-fp8.safetensors) |
| **2.3** | `distilled` | ![int8tensormixed][badge-int8tensormixed] | 29.1 GB | [![][gh-Winnougan]](https://huggingface.co/Winnougan/LTX-2.3-INT8/resolve/main/ltx-2.3-22b-distilled-int8tensormixed.safetensors) |
| **2.3** | `distilled` | ![nvfp4][badge-nvfp4] | 17.6 GB | [![][gh-Winnougan]](https://huggingface.co/Winnougan/LTX-2.3-INT8/resolve/main/ltx-2.3-22b-distilled_transformer_only_NVFP4.safetensors) |
| **2.3** | `distilled` | ![mxfp8mixed][badge-mxfp8mixed] | 29.7 GB | [![][gh-silveroxides]](https://huggingface.co/silveroxides/LTX-2.3-Quants/resolve/main/ltx-2.3-22b-distilled-mxfp8mixed.safetensors) |
| **2.3** | `distilled 1.1` | ![bf16][badge-bf16] | 46.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-22b-distilled-1.1.safetensors) |
| **2.3** | `ltx23_srx fp8_e4m3 experimental` | ![fp8][badge-fp8] | 21.97 GB | [![][gh-SOLRICKS]](https://huggingface.co/SOLRICKS/ltx23_srx_fp8_e4m3_experimental/resolve/main/ltx23_srx_fp8_e4m3_experimental.safetensors) |
| | | | | |
| **2** | `ltx-2-19b dev` | ![bf16][badge-bf16] | 43.3 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-dev.safetensors) |
| **2** | `ltx-2-19b dev` | ![fp8][badge-fp8] | 27.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-dev-fp8.safetensors) |
| **2** | `ltx-2-19b dev` | ![fp4][badge-fp4] | 20 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-dev-fp4.safetensors) |
| **2** | `ltx-2-19b distilled` | ![bf16][badge-bf16] | 43.3 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-distilled.safetensors) |
| **2** | `ltx-2-19b distilled` | ![fp8][badge-fp8] | 27.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-distilled-fp8.safetensors) |
| **2** | `ltx-2-19b distilled` | ![nvfp4][badge-nvfp4] | 20 GB | [![](https://img.shields.io/badge/szwagros-lightgrey?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co/szwagros/ltx-2-dist-nvfp4/resolve/main/ltx-2-19b-distilled-nvfp4-fixed-calibrated.safetensors) |

Quantized to fp8_e5m2 to support older Triton with older Pytorch on 30 series GPUs. For WangGP in Pinokio

| Ver | Name | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2** | `ltx-2-19b dev` | ![fp8_e5m2](https://img.shields.io/badge/fp8__e5m2-fe7d37?style=flat-square) | 27.1 GB | [![](https://img.shields.io/badge/progmars-lightgrey?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co/progmars/ltx-2-19b-dev-fp8_e5m2) |


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
| `distilled v1.1` | `36` | — | 739 MB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments/resolve/main/ltx-2.3-22b-distilled-lora-1.1_fro90_ceil36.safetensors) |
| `distilled v1.1` | `72` | condsafe | 662 MB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments/resolve/main/ltx-2.3-22b-distilled-lora-1.1_fro90_ceil72_condsafe.safetensors) |
| `distilled` | `72` | — | 1.4 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments/resolve/main/ltx-2.3-22b-distilled-lora-fro90_ceil72.safetensors) |
| `distilled v1.1` | `32` | condsafe | 363 MB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments/resolve/main/ltx-2.3-22b-distilled-lora-1.1_fro90_ceil32_condsafe.safetensors) |
| `distilled v1.1` | `52` | condsafe | 464 MB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments/resolve/main/ltx-2.3-22b-distilled-lora-1.1_fro90_ceil52_condsafe.safetensors) |
| `distilled v1.1` | `72` | energy | 1.6 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments/resolve/main/ltx-2.3-22b-distilled-lora-1.1_rank72_energy.safetensors) |
| `distilled v1.1` | `96` | energy | 2.2 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3_Distilled_Lora_1.1_Experiments/resolve/main/ltx-2.3-22b-distilled-lora-1.1_rank96_energy.safetensors) |

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
| **2.3** | `spatial-upscaler x2 1.0` | 996 MB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-spatial-upscaler-x2-1.0.safetensors) |
| **2.3** | `spatial-upscaler x1.5 1.0` | 1.09 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-spatial-upscaler-x1.5-1.0.safetensors) |
| | | | |
| **2** | `spatial-upscaler x2 1.0` | 1.05 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-spatial-upscaler-x2-1.0.safetensors) |


<p id="ckpt-temporal-upscaler" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ Temporal Upscaler

Required for current two-stage pipeline implementations in this repository. Download to `COMFYUI_ROOT_FOLDER/models/latent_upscale_models` folder.

| Ver | Name | Size | Download |
| :--- | :--- | :--- | :--- |
| **2.3** | `temporal-upscaler x2 1.0` | 262 MB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-temporal-upscaler-x2-1.0.safetensors) |
| | | | |
| **2** | `temporal-upscaler x2 1.0` | 262 MB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-temporal-upscaler-x2-1.0.safetensors) |

<p id="merges" align="center">══════════════════════════════════</p>

### ▣ Merges

Custom merged models combining multiple control signals or specialized configurations.

| Ver | Name | Description | Download |
| :--- | :--- | :--- | :--- |
| **2.3** | `ltx-2.3-22b-distilled-1.1-fused-union-control` | Merged model combining Canny, Depth, and Pose control signals for unified control | [![](https://img.shields.io/badge/linoyts-lightgrey?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co/linoyts/ltx-2.3-22b-distilled-1.1-fused-union-control) |

<p id="finetunes" align="center">══════════════════════════════════</p>

### ▣ Finetunes

Community finetuned models based on LTX-2.3 with specialized improvements and optimizations. Each finetune family may include a backbone checkpoint, low-VRAM component splits, GGUF quants, and merged or extracted LoRAs. Variant cell links go directly to the resolve/main safetensors/gguf file when a single canonical asset covers the row.

<a id="finetune-dasiwa"></a>

#### ❖ DaSiWa

High-performance LoRA-integrated checkpoint family based on LTX 2.3. Includes distilled (4-step) and non-distilled (20-30 step) variants. Recommended sampler: Euler + Simple/Normal/Linear_Quadratic.

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **2.3** | Distilled | `Treasurechest V1` | ![fp8][badge-fp8] | 19.58 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Distilled/FP8/v01/DasiwaLTX23Lightspeed_treasurechestV1.safetensors) |
| **2.3** | Distilled | `Solsticecoin V2` | ![fp8][badge-fp8] | 28.06 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Distilled/FP8/v03/DasiwaLTX23_solsticecoinV2-fp8.safetensors) |
| **2.3** | Distilled | `Dragonleap V4` | ![int4mixedtensorwise][badge-int4mixedtensorwise] | 17.10 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Distilled/DasiwaLTX23_dragonleapV4-INT4%20ConvRot.safetensors) |
| **2.3** | Distilled | `Dragonleap V4` | ![int8tensormixed][badge-int8tensormixed] | 25.73 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Distilled/DasiwaLTX23_dragonleapV4-INT8%20ConvRot.safetensors) |
| **2.3** | Non-Distilled | `GoldenLace V3` | ![fp8][badge-fp8] | 27.16 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/FP8/v03/DasiwaLTX23_goldenLaceV3-fp8.safetensors) |
| **2.3** | Non-Distilled | `GoldenLace V3` | ![nvfp4][badge-nvfp4] | 20.24 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/NVFP4/v03/DasiwaLTX23_goldenLaceV3-fp4.safetensors) |
| **2.3** | Non-Distilled GGUF | `GoldenLace V3` | ![Q2_K][badge-Q2_K] | 7.92 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/GGUF/v03/DasiwaLTX23_goldenLaceV3-Q2_K.gguf) |
| **2.3** | Non-Distilled GGUF | `GoldenLace V3` | ![Q3_K_M][badge-Q3_K_M] | 9.87 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/GGUF/v03/DasiwaLTX23_goldenLaceV3-Q3_K_M.gguf) |
| **2.3** | Non-Distilled GGUF | `GoldenLace V3` | ![Q4_K_M][badge-Q4_K_M] | 12.41 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/GGUF/v03/DasiwaLTX23_goldenLaceV3-Q4_K_M.gguf) |
| **2.3** | Non-Distilled GGUF | `GoldenLace V3` | ![Q5_K_M][badge-Q5_K_M] | 14.81 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/GGUF/v03/DasiwaLTX23_goldenLaceV3-Q5_K_M.gguf) |
| **2.3** | Non-Distilled GGUF | `GoldenLace V3` | ![Q6_K][badge-Q6_K] | 17.35 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/GGUF/v03/DasiwaLTX23_goldenLaceV3-Q6_K.gguf) |
| **2.3** | Non-Distilled GGUF | `GoldenLace V3` | ![Q8_0][badge-Q8_0] | 21.99 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Non-Distilled/GGUF/v03/DasiwaLTX23_goldenLaceV3-Q8_0.gguf) |

**DaSiWa extracted LoRA:**

| Build | Name | LoRA Rank | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| DMD v2 audio | `LTX2.3_DMD_v2_avgrank86_audio160_L80-D20` | 86 (audio 160) | 2.16 GB | [![DaSiWa][gh-DaSiWa]](https://huggingface.co/darksidewalker/DaSiWa-LTX2.3/resolve/main/Lora/LTX2.3_DMD_v2_avgrank86_audio160_L80-D20.safetensors) |

<p id="finetune-10eros" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ 10Eros

I2V-optimised merge using layer scaled merges at different steps. Not a straight weight merge — behaves much nicer than standard LoRA loading and respects prompts.

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **2.3** | Full | `10Eros v1` | ![bf16][badge-bf16] | 44.0 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1_bf16.safetensors) |
| **2.3** | Full | `10Eros v1` | ![fp8][badge-fp8] | 27.8 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1-fp8mixed_learned.safetensors) |
| **2.3** | transformer-only | `10Eros v1` | ![fp8][badge-fp8] | 28.2 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1_fp8_transformer.safetensors) |
| **2.3** | Full | `10Eros v1.2` | ![bf16][badge-bf16] | 44.0 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1.2_bf16.safetensors) |
| **2.3** | Full | `10Eros v1.2` | ![fp8][badge-fp8] | 32.7 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1.2_fp8mixed_learned.safetensors) |
| **2.3** | Full | `10Eros v1.3` | ![bf16][badge-bf16] | 44.0 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1.3_bf16.safetensors) |
| **2.3** | Full | `10Eros v1.3` | ![fp8][badge-fp8] | 27.8 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1.3_fp8mixed_learned.safetensors) |
| **2.3** | Full | `10Eros v1.4` | ![bf16][badge-bf16] | 44.0 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1.4_bf16.safetensors) |
| **2.3** | Full | `10Eros v1.4` | ![fp8][badge-fp8] | 27.8 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/10Eros_v1.4_fp8mixed_learned.safetensors) |
| **2.3** | Full | `10Eros v1.4` | ![int8tensormixed][badge-int8tensormixed] | 27.8 GB | [![TenStrip][gh-TenStrip]](https://huggingface.co/TenStrip/LTX2.3-10Eros/resolve/main/INT8%20diffusion_models/10Eros_v1.4_DMD_int8_convrot.safetensors) |

◦ **10Eros GGUF** — vantagewithai low-VRAM quants

<details>
  <summary>vantagewithai/LTX2.3-10Eros-GGUF</summary>

[`vantagewithai/LTX2.3-10Eros-GGUF`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF) — v1

| Quant | Size | Download |
| :--- | :---: | :--- |
| ![Q3_K_M][badge-Q3_K_M] | 10.36 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q3_K_M.gguf) |
| ![Q3_K_S][badge-Q3_K_S] | 9.63 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q3_K_S.gguf) |
| ![Q4_0][badge-Q4_0] | 12.09 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q4_0.gguf) |
| ![Q4_1][badge-Q4_1] | 12.95 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q4_1.gguf) |
| ![Q4_K_M][badge-Q4_K_M] | 13.31 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q4_K_M.gguf) |
| ![Q4_K_S][badge-Q4_K_S] | 12.29 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q4_K_S.gguf) |
| ![Q5_0][badge-Q5_0] | 14.21 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q5_0.gguf) |
| ![Q5_1][badge-Q5_1] | 15.07 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q5_1.gguf) |
| ![Q5_K_M][badge-Q5_K_M] | 15.03 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q5_K_M.gguf) |
| ![Q5_K_S][badge-Q5_K_S] | 14.01 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q5_K_S.gguf) |
| ![Q6_K][badge-Q6_K] | 16.55 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q6_K.gguf) |
| ![Q8_0][badge-Q8_0] | 21.19 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-GGUF/resolve/main/10Eros_v1-Q8_0.gguf) |

</details>

<details>
  <summary>vantagewithai/LTX2.3-10Eros-1.2-GGUF</summary>

[`vantagewithai/LTX2.3-10Eros-1.2-GGUF`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF) — v1.2 — **Note:** files are named `10Eros_v1.210Eros_v1.2-…gguf` (upstream double-stamp glitch); we link verbatim.

| Quant | Size | Download |
| :--- | :---: | :--- |
| ![Q3_K_M][badge-Q3_K_M] | 10.36 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q3_K_M.gguf) |
| ![Q3_K_S][badge-Q3_K_S] | 9.63 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q3_K_S.gguf) |
| ![Q4_0][badge-Q4_0] | 12.09 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q4_0.gguf) |
| ![Q4_1][badge-Q4_1] | 12.95 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q4_1.gguf) |
| ![Q4_K_M][badge-Q4_K_M] | 13.31 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q4_K_M.gguf) |
| ![Q4_K_S][badge-Q4_K_S] | 12.29 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q4_K_S.gguf) |
| ![Q5_0][badge-Q5_0] | 14.21 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q5_0.gguf) |
| ![Q5_1][badge-Q5_1] | 15.07 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q5_1.gguf) |
| ![Q5_K_M][badge-Q5_K_M] | 15.03 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q5_K_M.gguf) |
| ![Q5_K_S][badge-Q5_K_S] | 14.01 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q5_K_S.gguf) |
| ![Q6_K][badge-Q6_K] | 16.55 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q6_K.gguf) |
| ![Q8_0][badge-Q8_0] | 21.19 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-GGUF/resolve/main/10Eros_v1.210Eros_v1.2-Q8_0.gguf) |

</details>

<details>
  <summary>vantagewithai/LTX2.3-10Eros-1.3-GGUF</summary>

[`vantagewithai/LTX2.3-10Eros-1.3-GGUF`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF) — v1.3

| Quant | Size | Download |
| :--- | :---: | :--- |
| ![Q3_K_M][badge-Q3_K_M] | 10.36 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q3_K_M.gguf) |
| ![Q3_K_S][badge-Q3_K_S] | 9.63 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q3_K_S.gguf) |
| ![Q4_0][badge-Q4_0] | 12.09 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q4_0.gguf) |
| ![Q4_1][badge-Q4_1] | 12.95 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q4_1.gguf) |
| ![Q4_K_M][badge-Q4_K_M] | 13.31 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q4_K_M.gguf) |
| ![Q4_K_S][badge-Q4_K_S] | 12.29 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q4_K_S.gguf) |
| ![Q5_0][badge-Q5_0] | 14.21 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q5_0.gguf) |
| ![Q5_1][badge-Q5_1] | 15.07 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q5_1.gguf) |
| ![Q5_K_M][badge-Q5_K_M] | 15.03 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q5_K_M.gguf) |
| ![Q5_K_S][badge-Q5_K_S] | 14.01 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q5_K_S.gguf) |
| ![Q6_K][badge-Q6_K] | 16.55 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q6_K.gguf) |
| ![Q8_0][badge-Q8_0] | 21.19 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-GGUF/resolve/main/10Eros_v1.3-Q8_0.gguf) |

</details>

<details>
  <summary>vantagewithai/LTX2.3-10Eros-1.4-GGUF</summary>

[`vantagewithai/LTX2.3-10Eros-1.4-GGUF`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF) — v1.4 (latest)

| Quant | Size | Download |
| :--- | :---: | :--- |
| ![Q3_K_M][badge-Q3_K_M] | 10.36 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q3_K_M.gguf) |
| ![Q3_K_S][badge-Q3_K_S] | 9.63 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q3_K_S.gguf) |
| ![Q4_0][badge-Q4_0] | 12.09 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q4_0.gguf) |
| ![Q4_1][badge-Q4_1] | 12.95 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q4_1.gguf) |
| ![Q4_K_M][badge-Q4_K_M] | 13.31 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q4_K_M.gguf) |
| ![Q4_K_S][badge-Q4_K_S] | 12.29 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q4_K_S.gguf) |
| ![Q5_0][badge-Q5_0] | 14.21 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q5_0.gguf) |
| ![Q5_1][badge-Q5_1] | 15.07 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q5_1.gguf) |
| ![Q5_K_M][badge-Q5_K_M] | 15.03 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q5_K_M.gguf) |
| ![Q5_K_S][badge-Q5_K_S] | 14.01 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q5_K_S.gguf) |
| ![Q6_K][badge-Q6_K] | 16.55 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q6_K.gguf) |
| ![Q8_0][badge-Q8_0] | 21.19 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-GGUF/resolve/main/10Eros_v1.4-Q8_0.gguf) |

</details>

◦ **10Eros Splits**
<details>
  <summary>per-version component split</summary>

[`vantagewithai/LTX2.3-10Eros-Split`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-Split) — v1
| Component | Precision | Size | Download |
| :--- | :---: | :---: | :--- |
| Model | ![bf16][badge-bf16] | 41.03 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-Split/resolve/main/model/10Eros_v1_bf16_model.safetensors) |
| Model | ![fp8][badge-fp8] | 24.45 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-Split/resolve/main/model/10Eros_v1_fp8_model.safetensors) |
| VAE | — | 1.42 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-Split/resolve/main/vae/10Eros_v1_vae.safetensors) |
| Audio VAE | — | 364.86 MB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-Split/resolve/main/audio_vae/10Eros_v1_audio_vae.safetensors) |
| Text encoder | — | 2.26 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-Split/resolve/main/text_encoder/10Eros_v1_text_encoder.safetensors) |

[`vantagewithai/LTX2.3-10Eros-1.2-Split`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-Split) — v1.2
| Component | Precision | Size | Download |
| :--- | :---: | :---: | :--- |
| Model | ![bf16][badge-bf16] | 41.03 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-Split/resolve/main/model/10Eros_v1.2_bf16_model.safetensors) |
| Model | ![fp8][badge-fp8] | 29.49 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-Split/resolve/main/model/10Eros_v1.2_fp8mixed_learned_model.safetensors) |
| VAE | — | 1.42 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-Split/resolve/main/vae/10Eros_v1.2_vae.safetensors) |
| Audio VAE | — | 364.86 MB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-Split/resolve/main/audio_vae/10Eros_v1.2_audio_vae.safetensors) |
| LoRA (bundled) | — | 662.07 MB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.2-Split/resolve/main/lora/ltx-2.3-22b-distilled-lora-1.1_fro90_ceil72_condsafe.safetensors) |

[`vantagewithai/LTX2.3-10Eros-1.3-Split`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-Split) — v1.3
| Component | Precision | Size | Download |
| :--- | :---: | :---: | :--- |
| Model | ![bf16][badge-bf16] | 41.03 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-Split/resolve/main/model/10Eros_v1.3_bf16_model.safetensors) |
| Model | ![fp8][badge-fp8] | 24.45 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-Split/resolve/main/model/10Eros_v1.3_fp8mixed_learned_model.safetensors) |
| VAE | — | 1.42 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-Split/resolve/main/vae/10Eros_v1.3_vae.safetensors) |
| Audio VAE | — | 364.86 MB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-Split/resolve/main/audio_vae/10Eros_v1.3_audio_vae.safetensors) |
| Text encoder | — | 2.26 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.3-Split/resolve/main/text_encoder/10Eros_v1.3_text_encoder.safetensors) |

[`vantagewithai/LTX2.3-10Eros-1.4-Split`](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-Split) — v1.4 (latest)
| Component | Precision | Size | Download |
| :--- | :---: | :---: | :--- |
| Model | ![bf16][badge-bf16] | 41.03 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-Split/resolve/main/model/10Eros_v1.4_bf16_model.safetensors) |
| Model | ![fp8][badge-fp8] | 24.45 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-Split/resolve/main/model/10Eros_v1.4_fp8mixed_learned_model.safetensors) |
| VAE | — | 1.42 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-Split/resolve/main/vae/10Eros_v1.4_vae.safetensors) |
| Audio VAE | — | 364.86 MB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-Split/resolve/main/audio_vae/10Eros_v1.4_audio_vae.safetensors) |
| Text encoder | — | 2.26 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX2.3-10Eros-1.4-Split/resolve/main/text_encoder/10Eros_v1.4_text_encoder.safetensors) |


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

<p id="finetune-sulphur" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ Sulphur-2-base

Repo: [`SulphurAI/Sulphur-2-base`](https://huggingface.co/SulphurAI/Sulphur-2-base) — uncensored video generation model based on LTX 2.3 with built-in prompt enhancer. Merge base for 10Eros. T2V + I2V native.

◦ **Main video model**

| Ver | Build | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.3** | dev | ![bf16][badge-bf16] | 44.0 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/sulphur_dev_bf16.safetensors) |
| **2.3** | dev | ![fp8][badge-fp8] | 27.8 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/sulphur_dev_fp8mixed.safetensors) |
| **2.3** | distil | ![bf16][badge-bf16] | 44.0 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/sulphur_distil_bf16.safetensors) |
| **2.3** | distil | ![fp8][badge-fp8] | 27.8 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/Civitai/Sulphur-2-distilled-fp8/resolve/main/sulphur_distil_fp8mixed.safetensors) |
| **2.3** | distil | ![nvfp4][badge-nvfp4] | 18.6 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/coolthor/Sulphur-2-distilled-NVFP4/resolve/main/sulphur_distil_nvfp4.safetensors) |

◦ **vantagewithai component split** — [`vantagewithai/Sulphur-2-Base-Split`](https://huggingface.co/vantagewithai/Sulphur-2-Base-Split)

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| model (`sulphur_dev_bf16_model`) | ![bf16][badge-bf16] | 40.06 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/Sulphur-2-Base-Split/resolve/main/model/sulphur_dev_bf16_model.safetensors) |
| model (`sulphur_dev_model_fp8mixed`) | ![fp8][badge-fp8] | 23.87 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/Sulphur-2-Base-Split/resolve/main/model/sulphur_dev_model_fp8mixed.safetensors) |
| model (`sulphur_distil_bf16_model`) | ![bf16][badge-bf16] | 40.06 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/Sulphur-2-Base-Split/resolve/main/model/sulphur_distil_bf16_model.safetensors) |
| vae | — | 1.38 GB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/Sulphur-2-Base-Split/resolve/main/vae/sulphur_vae.safetensors) |
| audio_vae | — | 348.0 MB | [![vantagewithai][gh-vantagewithai]](https://huggingface.co/vantagewithai/Sulphur-2-Base-Split/resolve/main/audio_vae/sulphur_audio_vae.safetensors) |

<details>
  <summary>Abiray GGUF quants</summary>

◦ **Abiray GGUF quants** — [`Abiray/Sulphur-2-base-GGUF`](https://huggingface.co/Abiray/Sulphur-2-base-GGUF)

| Build | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| sulphur_dev | ![bf16][badge-bf16] | 40.09 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev_bf16.gguf) |
| sulphur_dev | ![Q3_K_M][badge-Q3_K_M] | 10.36 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q3_K_M.gguf) |
| sulphur_dev | ![Q3_K_S][badge-Q3_K_S] | 9.63 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q3_K_S.gguf) |
| sulphur_dev | ![Q4_0][badge-Q4_0] | 12.09 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q4_0.gguf) |
| sulphur_dev | ![Q4_K_M][badge-Q4_K_M] | 13.31 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q4_K_M.gguf) |
| sulphur_dev | ![Q4_K_S][badge-Q4_K_S] | 12.29 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q4_K_S.gguf) |
| sulphur_dev | ![Q5_0][badge-Q5_0] | 14.21 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q5_0.gguf) |
| sulphur_dev | ![Q5_K_M][badge-Q5_K_M] | 15.04 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q5_K_M.gguf) |
| sulphur_dev | ![Q5_K_S][badge-Q5_K_S] | 14.01 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q5_K_S.gguf) |
| sulphur_dev | ![Q6_K][badge-Q6_K] | 16.55 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q6_K.gguf) |
| sulphur_dev | ![Q8_0][badge-Q8_0] | 21.19 GB | [![Abiray][gh-Abiray]](https://huggingface.co/Abiray/Sulphur-2-base-GGUF/resolve/main/sulphur_dev-Q8_0.gguf) |


</details>

◦ **Sulphur LoRAs**

| Ver | Build | Size | Download |
| :--- | :--- | :---: | :---: |
| **2.3** | `sulphur_lora_rank_768` | 9.79 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/sulphur_lora_rank_768.safetensors) |
| **2.3** (experimental) | `sulphur_experimental_lora_v1` | 13.87 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/experimental/sulphur_experimental_lora_v1.safetensors) |

◦ **Prompt Enhancer**

| Variant | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| Censored | ![bf16][badge-bf16] | 879.01 MB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/prompt_enhancer/mmproj-BF16.gguf) |
| Censored | ![Q8_0][badge-Q8_0] | 9.09 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/prompt_enhancer/sulphur_prompt_enhancer_model-q8_0.gguf) |
| Uncensored | ![bf16][badge-bf16] | 879.01 MB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/prompt_enhancer_uncensored/mmproj-prompt_enhancer_uncensored.gguf) |
| Uncensored | ![Q8_0][badge-Q8_0] | 9.33 GB | [![Sulphur][gh-SulphurAI]](https://huggingface.co/SulphurAI/Sulphur-2-base/resolve/main/prompt_enhancer_uncensored/prompt_enhancer_uncensored-q8_0.gguf) |

<p id="finetune-joyai-echo-surgical" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ JoyAI-Echo Surgical

Surgical finetune based on [jdopensource/JoyAI-Echo](https://huggingface.co/jdopensource/JoyAI-Echo) by joeygambino. Combined "echoVid + ltxAud" surgical variant — jointly fine-tuned for both video generation and audio on top of LTX-2.3. A LoRA extracted from JoyAI-Echo (TenStrip's `LTX2.3_JoyAI_Lora_Extracted`) is listed separately under `### ▣ Special`.

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **2.3** | unsplit (full DiT) | `echoVid-ltxAud surgical` | ![bf16][badge-bf16] | 42.97 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical/resolve/main/ltx23_echoVid-ltxAud_surgical_bf16.safetensors) |
| **2.3** | unsplit (full DiT) | `echoVid-ltxAud surgical` | ![fp8][badge-fp8] | 23.41 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical/resolve/main/ltx23_echoVid-ltxAud_surgical_fp8.safetensors) |
| **2.3** | unsplit (full DiT) | `echoVid-ltxAud surgical` | ![int8tensormixed][badge-int8tensormixed] | 27.15 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical-int8/resolve/main/ltx23_echoVid-ltxAud_surgical_int8_convrot.safetensors) |
| **2.3** | transformer-only | `echoVid-ltxAud surgical` | ![int8tensormixed][badge-int8tensormixed] | 26.07 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical-int8/resolve/main/ltx23_echoVid-ltxAud_surgical_int8_convrot_transformer_only.safetensors) |

◦ **JoyAI-Echo Surgical — GGUF (low-VRAM quants)**

<details>
  <summary>joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical-gguf</summary>

[`joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical-gguf`](https://huggingface.co/joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical-gguf) — Surgical DiT GGUF quants by joeygambino.

| Ver | Build | Name | Precision | Size | Download |
| :--- | :--- | :--- | :---: | :---: | :---: |
| **2.3** | GGUF | `echoVid-ltxAud surgical` | ![Q5_0][badge-Q5_0] | 15.54 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical-gguf/resolve/main/LTX23-echoVid-ltxAud-Surgical-DiT-Q5_0.gguf) |
| **2.3** | GGUF | `echoVid-ltxAud surgical` | ![Q8_0][badge-Q8_0] | 23.13 GB | [![joeygambino][gh-joeygambino]](https://huggingface.co/joeygambino/joyai-echo-ltx23-echoVid-ltxAud-surgical-gguf/resolve/main/LTX23-echoVid-ltxAud-Surgical-DiT-Q8_0.gguf) |

</details>

<p id="finetune-pinkcherry" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ PinkCherry NSFW

| Variant | Description | Download |
| :--- | :--- | :--- |
| v1.3 dev bf16 | PinkCherry uncensored NSFW LTX-2.3 finetune; v1.3 BF16 dev. Pairs with the official LTX-2.3 distilled LoRA 384. NSFW content only — do not use for clean content. | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.3/SexGod_PinkCherry_dev_bf16_LTX23_v1_3.safetensors) |
| v1.5 dev bf16 | PinkCherry v1.5 BF16 — newer training pass than v1.3 with updated workflow. | [![PinkCherry][gh-SexGod1979]](https://huggingface.co/SexGod1979/PinkCherry_NSFW_LTX23/resolve/main/v1.5/SexGod_PinkCherry_dev_bf16_LTX23_v1_5.safetensors) |

#### ❖ Elastic

Elastic is a TensorRT-engine distribution of a LoRA-integrated distilled FP8 T2V variant of LTX-2.3, packaged by [TheStageAI](https://huggingface.co/TheStageAI/Elastic-LTX-2.3) as `.qlip` shard files for H100 GPUs.

| Build | Name | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| distil + LoRA T2V | `Elastic — H100` | fp8 | ~19 GB (49 `.qlip` shards) | [![TheStageAI][gh-TheStageAI]](https://huggingface.co/TheStageAI/Elastic-LTX-2.3/tree/main/models/H100/ltx-2.3-22b-distilled-fp8-t2v_lora) |

<p id="finetune-spatialav2av" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ SpatialAV2AV (BingoG)

Publicly-released audio→audio-video training checkpoints from [BingoG/LTX-2-SpatialAV2AV-Checkpoints](https://huggingface.co/BingoG/LTX-2-SpatialAV2AV-Checkpoints) for spatial-audio conditioned video generation. Two curriculum layouts (`E4` Core Dual + Dynamic; `E6` reserved for Full) at 480p cap, 113 frames at 25 fps.

| Curriculum | Step | Size | Download |
| :--- | :---: | :---: | :---: |
| E4 Core (Dual + Dynamic) | 400  | 36.22 GB | [![BingoG][gh-BingoG]](https://huggingface.co/BingoG/LTX-2-SpatialAV2AV-Checkpoints/resolve/main/E4/step_00400/model_weights_step_00400.safetensors) |
| E4 Core (Dual + Dynamic) | 1000 | 36.22 GB | [![BingoG][gh-BingoG]](https://huggingface.co/BingoG/LTX-2-SpatialAV2AV-Checkpoints/resolve/main/E4/step_01000/model_weights_step_01000.safetensors) |
| E6 Full                  | 1000 | 36.22 GB | [![BingoG][gh-BingoG]](https://huggingface.co/BingoG/LTX-2-SpatialAV2AV-Checkpoints/resolve/main/E6/step_01000/model_weights_step_01000.safetensors) |

*Note: these are intermediate training checkpoints, not inference-ready models — useful for fine-tuning experiments and reproducibility only.*

<p id="gguf" align="center">══════════════════════════════════</p>


### ▣ GGUF Quantized Models
These models are optimized for lower memory usage. Note that in ComfyUI, these are typically loaded as transformer-only models.

<details>
  <summary>QuantStack</summary>

  #### [QuantStack LTX-2.3](https://huggingface.co/QuantStack/LTX-2.3-GGUF)

| Model | Quant | Size | Download |
| :--- | :---: | :---: | :---: |
| ltx-2.3-22b | ![Q2_K][badge-Q2_K] | 12.4 GB | [dev](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-dev/LTX-2.3-dev-Q2_K.gguf) ┊ [distilled](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled/LTX-2.3-distilled-Q2_K.gguf) ┊ [distilled-1.1](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled-1.1/LTX-2.3-22B-distilled-1.1-Q2_K.gguf) |
| ltx-2.3-22b | ![Q3_K_M][badge-Q3_K_M] | 14.7 GB | [dev](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-dev/LTX-2.3-dev-Q3_K_M.gguf) ┊ [distilled](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled/LTX-2.3-distilled-Q3_K_M.gguf) ┊ [distilled-1.1](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled-1.1/LTX-2.3-22B-distilled-1.1-Q3_K_M.gguf) |
| ltx-2.3-22b | ![Q3_K_S][badge-Q3_K_S] | 14 GB | [dev](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-dev/LTX-2.3-dev-Q3_K_S.gguf) ┊ [distilled](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled/LTX-2.3-distilled-Q3_K_S.gguf) ┊ [distilled-1.1](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled-1.1/LTX-2.3-22B-distilled-1.1-Q3_K_S.gguf) |
| ltx-2.3-22b | ![Q4_K_M][badge-Q4_K_M] | 17.8 GB | [dev](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-dev/LTX-2.3-dev-Q4_K_M.gguf) ┊ [distilled](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled/LTX-2.3-distilled-Q4_K_M.gguf) ┊ [distilled-1.1](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled-1.1/LTX-2.3-22B-distilled-1.1-Q4_K_M.gguf) |
| ltx-2.3-22b | ![Q4_K_S][badge-Q4_K_S] | 16.7 GB | [dev](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-dev/LTX-2.3-dev-Q4_K_S.gguf) ┊ [distilled](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled/LTX-2.3-distilled-Q4_K_S.gguf) ┊ [distilled-1.1](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled-1.1/LTX-2.3-22B-distilled-1.1-Q4_K_S.gguf) |
| ltx-2.3-22b | ![Q5_K_M][badge-Q5_K_M] | 19.4 GB | [dev](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-dev/LTX-2.3-dev-Q5_K_M.gguf) ┊ [distilled](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled/LTX-2.3-distilled-Q5_K_M.gguf) ┊ [distilled-1.1](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled-1.1/LTX-2.3-22B-distilled-1.1-Q5_K_M.gguf) |
| ltx-2.3-22b | ![Q5_K_S][badge-Q5_K_S] | 18.5 GB | [dev](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-dev/LTX-2.3-dev-Q5_K_S.gguf) ┊ [distilled](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled/LTX-2.3-distilled-Q5_K_S.gguf) ┊ [distilled-1.1](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled-1.1/LTX-2.3-22B-distilled-1.1-Q5_K_S.gguf) |
| ltx-2.3-22b | ![Q6_K][badge-Q6_K] | 21 GB | [dev](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-dev/LTX-2.3-dev-Q6_K.gguf) ┊ [distilled](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled/LTX-2.3-distilled-Q6_K.gguf) ┊ [distilled-1.1](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled-1.1/LTX-2.3-22B-distilled-1.1-Q6_K.gguf) |
| ltx-2.3-22b | ![Q8_0][badge-Q8_0] | 25.5 GB | [dev](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-dev/LTX-2.3-dev-Q8_0.gguf) ┊ [distilled](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled/LTX-2.3-distilled-Q8_0.gguf) ┊ [distilled-1.1](https://huggingface.co/QuantStack/LTX-2.3-GGUF/resolve/main/LTX-2.3-distilled-1.1/LTX-2.3-22B-distilled-1.1-Q8_0.gguf) |

#### [QuantStack LTX-2](https://huggingface.co/QuantStack/LTX-2-GGUF)

| Model | Quant | Size | Download |
| :--- | :---: | :---: | :---: |
| LTX-2-dev | ![Q2_K][badge-Q2_K] | 8.03 GB | [![][gh-QuantStack]](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q2_K.gguf) |
| LTX-2-dev | ![Q3_K_M][badge-Q3_K_M] | 10.3 GB | [![][gh-QuantStack]](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q3_K_M.gguf) |
| LTX-2-dev | ![Q3_K_S][badge-Q3_K_S] | 9.57 GB | [![][gh-QuantStack]](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q3_K_S.gguf) |
| LTX-2-dev | ![Q4_K_M][badge-Q4_K_M] | 13.4 GB | [![][gh-QuantStack]](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q4_K_M.gguf) |
| LTX-2-dev | ![Q4_K_S][badge-Q4_K_S] | 12.3 GB | [![][gh-QuantStack]](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q4_K_S.gguf) |
| LTX-2-dev | ![Q5_K_M][badge-Q5_K_M] | 15 GB | [![][gh-QuantStack]](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q5_K_M.gguf) |
| LTX-2-dev | ![Q5_K_S][badge-Q5_K_S] | 14.2 GB | [![][gh-QuantStack]](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q5_K_S.gguf) |
| LTX-2-dev | ![Q6_K][badge-Q6_K] | 16.6 GB | [![][gh-QuantStack]](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q6_K.gguf) |
| LTX-2-dev | ![Q8_0][badge-Q8_0] | 21.1 GB | [![][gh-QuantStack]](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q8_0.gguf) |

</details>

<details>
  <summary>Unsloth </summary>

#### [Unsloth LTX-2.3 GGUF](https://huggingface.co/unsloth/LTX-2.3-GGUF)

| Model | Quant | Size | Download |
| :--- | :--- | :--- | :--- |
| ltx-2.3-22b | ![BF16][badge-BF16] | 42 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-BF16.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-BF16.gguf) |
| ltx-2.3-22b | ![F16][badge-F16] | 42 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-F16.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-F16.gguf) |
| ltx-2.3-22b | ![Q2_K][badge-Q2_K] | 8.28 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-Q2_K.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-Q2_K.gguf) |
| ltx-2.3-22b | ![Q3_K_M][badge-Q3_K_M] | 10.8 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-Q3_K_M.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-Q3_K_M.gguf) |
| ltx-2.3-22b | ![Q3_K_S][badge-Q3_K_S] | 9.95 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-Q3_K_S.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-Q3_K_S.gguf) |
| ltx-2.3-22b | ![Q4_0][badge-Q4_0] | 12.7 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-Q4_0.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-Q4_0.gguf) |
| ltx-2.3-22b | ![Q4_1][badge-Q4_1] | 13.8 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-Q4_1.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-Q4_1.gguf) |
| ltx-2.3-22b | ![Q4_K_M][badge-Q4_K_M] | 14.3 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-Q4_K_M.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-Q4_K_M.gguf) |
| ltx-2.3-22b | ![Q4_K_S][badge-Q4_K_S] | 13.1 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-Q4_K_S.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-Q4_K_S.gguf) |
| ltx-2.3-22b | ![Q5_0][badge-Q5_0] | 15.3 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-Q5_0.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-Q5_0.gguf) |
| ltx-2.3-22b | ![Q5_1][badge-Q5_1] | 16.3 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-Q5_1.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-Q5_1.gguf) |
| ltx-2.3-22b | ![Q5_K_M][badge-Q5_K_M] | 16.1 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-Q5_K_M.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-Q5_K_M.gguf) |
| ltx-2.3-22b | ![Q5_K_S][badge-Q5_K_S] | 15.2 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-Q5_K_S.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-Q5_K_S.gguf) |
| ltx-2.3-22b | ![Q6_K][badge-Q6_K] | 17.8 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-Q6_K.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-Q6_K.gguf) |
| ltx-2.3-22b | ![Q8_0][badge-Q8_0] | 22.8 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-Q8_0.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-Q8_0.gguf) |
| ltx-2.3-22b | ![UD-Q2_K][badge-UD-Q2_K] | 9.5 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-UD-Q2_K.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-UD-Q2_K.gguf) |
| ltx-2.3-22b | ![UD-Q3_K_M][badge-UD-Q3_K_M] | 13.5 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-UD-Q3_K_M.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-UD-Q3_K_M.gguf) |
| ltx-2.3-22b | ![UD-Q3_K_S](https://img.shields.io/badge/UD-Q3__K__S-fe7d37?style=flat-square) | 11.4 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-UD-Q3_K_S.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-UD-Q3_K_S.gguf) |
| ltx-2.3-22b | ![UD-Q4_K_M][badge-UD-Q4_K_M] | 16.5 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-UD-Q4_K_M.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-UD-Q4_K_M.gguf) |
| ltx-2.3-22b | ![UD-Q4_K_S][badge-UD-Q4_K_S] | 14.2 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-UD-Q4_K_S.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-UD-Q4_K_S.gguf) |
| ltx-2.3-22b | ![UD-Q5_K_M][badge-UD-Q5_K_M] | 18.3 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-UD-Q5_K_M.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-UD-Q5_K_M.gguf) |
| ltx-2.3-22b | ![UD-Q5_K_S](https://img.shields.io/badge/UD-Q5__K__S-97c00f?style=flat-square) | 16.3 GB | [dev](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/ltx-2.3-22b-dev-UD-Q5_K_S.gguf) ┊ [distilled](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled/ltx-2.3-22b-distilled-UD-Q5_K_S.gguf) |

#### [Unsloth LTX-2.3 GGUF - Distilled 1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/tree/main/distilled-1.1)

| Model | Quant | Size | Download |
| :--- | :--- | :--- | :--- |
| ltx-2.3-22b | ![BF16][badge-BF16] | 42 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-BF16.gguf) |
| ltx-2.3-22b | ![F16][badge-F16] | 42 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-F16.gguf) |
| ltx-2.3-22b | ![Q2_K][badge-Q2_K] | 7.94 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-Q2_K.gguf) |
| ltx-2.3-22b | ![Q3_K_M][badge-Q3_K_M] | 10.6 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-Q3_K_M.gguf) |
| ltx-2.3-22b | ![Q3_K_S][badge-Q3_K_S] | 9.74 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-Q3_K_S.gguf) |
| ltx-2.3-22b | ![Q4_K_M][badge-Q4_K_M] | 14.2 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-Q4_K_M.gguf) |
| ltx-2.3-22b | ![Q4_K_S][badge-Q4_K_S] | 13 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-Q4_K_S.gguf) |
| ltx-2.3-22b | ![Q5_K_M][badge-Q5_K_M] | 15.9 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-Q5_K_M.gguf) |
| ltx-2.3-22b | ![Q5_K_S][badge-Q5_K_S] | 15 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-Q5_K_S.gguf) |
| ltx-2.3-22b | ![Q6_K][badge-Q6_K] | 17.8 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-Q6_K.gguf) |
| ltx-2.3-22b | ![Q8_0][badge-Q8_0] | 22.8 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-Q8_0.gguf) |
| ltx-2.3-22b | ![UD-Q2_K][badge-UD-Q2_K] | 10.9 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-UD-Q2_K.gguf) |
| ltx-2.3-22b | ![UD-Q3_K_M][badge-UD-Q3_K_M] | 13.4 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-UD-Q3_K_M.gguf) |
| ltx-2.3-22b | ![UD-Q4_K_M][badge-UD-Q4_K_M] | 16.4 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-UD-Q4_K_M.gguf) |
| ltx-2.3-22b | ![UD-Q4_K_S][badge-UD-Q4_K_S] | 14.1 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-UD-Q4_K_S.gguf) |
| ltx-2.3-22b | ![UD-Q5_K_M][badge-UD-Q5_K_M] | 18.2 GB | [distilled-1.1](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/distilled-1.1/ltx-2.3-22b-distilled-1.1-UD-Q5_K_M.gguf) |

#### [Unsloth LTX-2 GGUF](https://huggingface.co/unsloth/LTX-2-GGUF)

| Model | Quant | Size | Download |
| :--- | :--- | :--- | :--- |
| ltx-2-19b-dev | ![BF16][badge-BF16] | 37.8 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-BF16.gguf) |
| ltx-2-19b-dev | ![F16][badge-F16] | 37.8 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-F16.gguf) |
| ltx-2-19b-dev | ![UD-Q2_K_L](https://img.shields.io/badge/UD-Q2__K__L-e05d44?style=flat-square) | 10.1 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-UD-Q2_K_L.gguf) |
| ltx-2-19b-dev | ![UD-Q2_K_XL](https://img.shields.io/badge/UD-Q2__K__XL-e05d44?style=flat-square) | 11.6 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-UD-Q2_K_XL.gguf) |
| ltx-2-19b-dev | ![Q2_K][badge-Q2_K] | 8.1 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q2_K.gguf) |
| ltx-2-19b-dev | ![Q3_K_L](https://img.shields.io/badge/Q3__K__L-fe7d37?style=flat-square) | 10.7 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q3_K_L.gguf) |
| ltx-2-19b-dev | ![Q3_K_M][badge-Q3_K_M] | 10.1 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q3_K_M.gguf) |
| ltx-2-19b-dev | ![Q3_K_S][badge-Q3_K_S] | 9.47 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q3_K_S.gguf) |
| ltx-2-19b-dev | ![Q4_0][badge-Q4_0] | 11.3 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q4_0.gguf) |
| ltx-2-19b-dev | ![Q4_1][badge-Q4_1] | 12.3 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q4_1.gguf) |
| ltx-2-19b-dev | ![Q4_K_M][badge-Q4_K_M] | 12.8 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q4_K_M.gguf) |
| ltx-2-19b-dev | ![Q4_K_S][badge-Q4_K_S] | 11.9 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q4_K_S.gguf) |
| ltx-2-19b-dev | ![Q5_0][badge-Q5_0] | 13.7 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q5_0.gguf) |
| ltx-2-19b-dev | ![Q5_1][badge-Q5_1] | 14.6 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q5_1.gguf) |
| ltx-2-19b-dev | ![Q5_K_M][badge-Q5_K_M] | 14.3 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q5_K_M.gguf) |
| ltx-2-19b-dev | ![Q5_K_S][badge-Q5_K_S] | 13.6 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q5_K_S.gguf) |
| ltx-2-19b-dev | ![Q6_K][badge-Q6_K] | 16 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q6_K.gguf) |
| ltx-2-19b-dev | ![Q8_0][badge-Q8_0] | 20.4 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q8_0.gguf) |


</details>

<details>
  <summary>Vantage</summary>

#### [Vantage AI GGUFs](https://huggingface.co/vantagewithai/)

| Model | Quant | Size | Download |
| :--- | :--- | :--- | :--- |
| ltx-2-19b-dev | ![Q3_K_M][badge-Q3_K_M] | 9.96 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q3_K_M.gguf) |
| ltx-2-19b-dev | ![Q3_K_S][badge-Q3_K_S] | 9.28 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q3_K_S.gguf) |
| ltx-2-19b-dev | ![Q4_0][badge-Q4_0] | 11.6 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q4_0.gguf) |
| ltx-2-19b-dev | ![Q4_1][badge-Q4_1] | 12.4 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q4_1.gguf) |
| ltx-2-19b-dev | ![Q4_K_M][badge-Q4_K_M] | 12.8 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q4_K_M.gguf) |
| ltx-2-19b-dev | ![Q4_K_S][badge-Q4_K_S] | 11.8 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q4_K_S.gguf) |
| ltx-2-19b-dev | ![Q5_0][badge-Q5_0] | 13.6 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q5_0.gguf) |
| ltx-2-19b-dev | ![Q5_1][badge-Q5_1] | 14.5 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q5_1.gguf) |
| ltx-2-19b-dev | ![Q5_K_M][badge-Q5_K_M] | 14.4 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q5_K_M.gguf) |
| ltx-2-19b-dev | ![Q5_K_S][badge-Q5_K_S] | 13.5 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q5_K_S.gguf) |
| ltx-2-19b-dev | ![Q6_K][badge-Q6_K] | 15.9 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q6_K.gguf) |
| ltx-2-19b-dev | ![Q8_0][badge-Q8_0] | 20.4 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q8_0.gguf) |
| ltx-2-19b-distilled | ![Q3_K_M][badge-Q3_K_M] | 9.96 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q3_K_M.gguf) |
| ltx-2-19b-distilled | ![Q3_K_S][badge-Q3_K_S] | 9.28 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q3_K_S.gguf) |
| ltx-2-19b-distilled | ![Q4_0][badge-Q4_0] | 11.6 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q4_0.gguf) |
| ltx-2-19b-distilled | ![Q4_1][badge-Q4_1] | 12.4 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q4_1.gguf) |
| ltx-2-19b-distilled | ![Q4_K_M][badge-Q4_K_M] | 12.8 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q4_K_M.gguf) |
| ltx-2-19b-distilled | ![Q4_K_S][badge-Q4_K_S] | 11.8 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q4_K_S.gguf) |
| ltx-2-19b-distilled | ![Q5_0][badge-Q5_0] | 13.6 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q5_0.gguf) |
| ltx-2-19b-distilled | ![Q5_1][badge-Q5_1] | 14.5 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q5_1.gguf) |
| ltx-2-19b-distilled | ![Q5_K_M][badge-Q5_K_M] | 14.4 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q5_K_M.gguf) |
| ltx-2-19b-distilled | ![Q5_K_S][badge-Q5_K_S] | 13.5 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q5_K_S.gguf) |
| ltx-2-19b-distilled | ![Q6_K][badge-Q6_K] | 15.9 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q6_K.gguf) |
| ltx-2-19b-distilled | ![Q8_0][badge-Q8_0] | 20.4 GB | [![][gh-vantagewithai]](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q8_0.gguf) |

</details>

#### Special Quantization: PolarQuant Q5

**LTX-2.3 (22B) — PolarQuant Q5** is a bit-packed quantization method using Hadamard-Rotated Lloyd-Max Quantization. It achieves optimal Gaussian weight quantization via Hadamard rotation, delivering near-lossless quality with significant size reduction.

<details>
  <summary>Specification</summary>

  <img  alt="image" src="https://github.com/user-attachments/assets/2f7e3300-aadf-447e-acd8-695fb1110a77" />

| Specification | Value |
|--------------|-------|
| Parameters | 22B |
| Transformer Blocks | 48 |
| Hidden Dimension | 4096 |
| Layers Quantized | 1,347 (of 5,947 total tensors) |

**Compression Statistics:**

| Component | Original Size | PQ5 Packed | Reduction |
|-----------|--------------|------------|----------|
| Transformer (1,347 layers) | 37 GB | 4.6 GB | **-88%** |
| VAE + Skip (4,600 layers) | 9.1 GB | 9.1 GB | BF16 kept |
| Upscalers | 1.3 GB | 1.3 GB | BF16 kept |
| **Total** | **46.2 GB** | **15 GB** | **-68%** |

<img alt="image" src="https://github.com/user-attachments/assets/5f833dc6-91b5-4aae-b33e-59e498fa5aa3" />


**Quality Metrics:**
- Cosine Similarity: **0.9986** (near-lossless)
- Download Size: **15 GB**
- Beats torchao INT4 on perplexity (PPL)

**Hardware Requirements:**

| GPU | VRAM | Status |
|-----|------|--------|
| A100 (80 GB) | 80 GB | Full speed |
| A100 (40 GB) | 40 GB | Recommended |
| RTX 4090 (24 GB) | 24 GB | With offloading |

**Key Features:**
- Mixed precision approach: transformer heavily quantized (-88%) while VAE remains BF16
- 5-bit bit-packed representation (Q5)
- 50-65% smaller than original with zero quality loss
- One-command setup with easy generation wrapper
</details>

| Model | Size | Download |
| :--- | :---: | :--- |
| `LTX-2.3-22B-PolarQuant-Q5` | 15 GB | [![](https://img.shields.io/badge/caiovicentino1-lightgrey?style=flat-square&logo=huggingface&logoColor=white)](https://huggingface.co/caiovicentino1/LTX-2.3-22B-PolarQuant-Q5) |

*Installation:* `pip install safetensors huggingface_hub scipy`
*ArXiv Reference:* [2603.29078](https://arxiv.org/abs/2603.29078)

<p id="text-encoder" align="center">◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆</p>

## ▓ Text Encoders

LTX-2 requires Gemma-3-12b variants. LTX-2.3 uses text projection layers.

### ▣ Comfy-Org Optimized Encoders

Official and optimized versions for ComfyUI.

| Model Name | Size | Download |
| :--- | :--- | :---: |
| `gemma_3_12B_it` | 24.4 GB | [![][gh-Comfy--Org]](https://huggingface.co/Comfy-Org/ltx-2/resolve/main/split_files/text_encoders/gemma_3_12B_it.safetensors?download=true) |
| `gemma_3_12B_it_fpmixed` | 13.7 GB | [![][gh-Comfy--Org]](https://huggingface.co/Comfy-Org/ltx-2/resolve/main/split_files/text_encoders/gemma_3_12B_it_fpmixed.safetensors?download=true) |
| `gemma_3_12B_it_fp8_scaled` | 13.2 GB | [![][gh-Comfy--Org]](https://huggingface.co/Comfy-Org/ltx-2/resolve/main/split_files/text_encoders/gemma_3_12B_it_fp8_scaled.safetensors?download=true) |
| `gemma_3_12B_it_fp4_mixed` |  9.5 GB | [![][gh-Comfy--Org]](https://huggingface.co/Comfy-Org/ltx-2/resolve/main/split_files/text_encoders/gemma_3_12B_it_fp4_mixed.safetensors?download=true) |
| `gemma_3_12B_it-int8tensormixed` | 13.2 GB | [![][gh-silveroxides]](https://huggingface.co/silveroxides/LTX-2.3-Quants/resolve/main/gemma_3_12B_it-int8tensormixed.safetensors) |
| `gemma_3_12B_it-int8mixedblockwise` | 13.6 GB | [![][gh-silveroxides]](https://huggingface.co/silveroxides/LTX-2.3-Quants/resolve/main/gemma_3_12B_it_int8mixedblockwise.safetensors) |
| `gemma_3_12B_it-int8mixedtensorwise` | 14.1 GB | [![][gh-silveroxides]](https://huggingface.co/silveroxides/LTX-2.3-Quants/resolve/main/gemma_3_12B_it_int8mixedtensorwise.safetensors) |
| `gemma_3_12B_it-int8tensormixed` | 13.2 GB | [![][gh-Winnougan]](https://huggingface.co/Winnougan/LTX-2.3-INT8/resolve/main/gemma_3_12B_it-int8tensormixed.safetensors) |
| `text_projection_fp8` | 1.16 GB | [![][gh-Winnougan]](https://huggingface.co/Winnougan/LTX-2.3-INT8/resolve/main/ltx-2.3_text_projection_fp8.safetensors) |

* `gemma_3_12B_it_fpmixed`: Experimental quant. Should be better than the fp8 scaled
* `gemma_3_12B_it_fp4_mixed`: 90% fp4 layers
**Note:** mxfp8mixed quantization requires a custom fork of ComfyUI-Kitchen with mxfp8 support. Standard ComfyUI setups don't.

<p id="enc-abliterated" align="center">· · · · · · · · · · · · · ·</p>

### ▣ Gemma-3-12b Abliterated

#### Why Choose Abliterated Encoders?

Standard Gemma models often incorporate safety alignment that "sanitizes" or weakens specific concepts within prompt embeddings. Even when the model doesn't explicitly refuse a request, this internal filtering can dilute creative intent. For LTX-2 video generation, using a standard encoder often results in:

* **Reduced Prompt Adherence:** Key stylistic or descriptive terms may be ignored or weakened.
* **Visual Softening:** Visual intensity and fine details are often "muted" to fit generic safety profiles.
* **Concept Dilution:** Complex or niche creative requests are subtly altered, leading to less faithful representations of your vision.

**Abliteration** bypasses these restrictive alignment layers, allowing the encoder to translate your prompts into embeddings with maximum fidelity. This ensures LTX-2 receives the most accurate and un-filtered instructions possible.

<details>
  <summary>Gemma-3-12b-Abliterated (FusionCow)</summary>

Fixed versions of the abliterated Gemma-3-12b-it model by [FusionCow](https://huggingface.co/FusionCow/Gemma-3-12b-Abliterated-LTX2), modified specifically for compatibility with LTX-2. The [original model](https://huggingface.co/mlabonne/gemma-3-12b-it-abliterated-v2)

| Model | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `Gemma ablit fixed` | ![bf16][badge-bf16] | 23.5 GB | [![][gh-FusionCow]](https://huggingface.co/FusionCow/Gemma-3-12b-Abliterated-LTX2/resolve/main/gemma_ablit_fixed_bf16.safetensors?download=true) |
| `Gemma ablit fixed` | ![fp8][badge-fp8] | 13.8 GB | [![][gh-FusionCow]](https://huggingface.co/FusionCow/Gemma-3-12b-Abliterated-LTX2/resolve/main/gemma_ablit_fixed_fp8.safetensors?download=true) |

</details>

<details>
  <summary>Sikaworld1990 Gemma-3-12b Abliterated</summary>

NVFP4 quantization variants by [Sikaworld1990](https://huggingface.co/Sikaworld1990) optimized for Blackwell GPUs.

| Model | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `Gemma-3-12b QAT Abliterated FP4` | ![NVFP4-HF](https://img.shields.io/badge/NVFP4--HF-6f42c1?style=flat-square) | 12.1 GB | [![][gh-Sikaworld1990]](https://huggingface.co/Sikaworld1990/gemma-3-12b-qat-abliterated-sikaworld-fp4-ltx2/resolve/main/Gemma3-12B-NVFP4-Sikaworld-HF.safetensors) |
| `Gemma-3-12b QAT Abliterated FP4` | ![NVFP4-Pure](https://img.shields.io/badge/NVFP4--Pure-6f42c1?style=flat-square) | 8.91 GB | [![][gh-Sikaworld1990]](https://huggingface.co/Sikaworld1990/gemma-3-12b-qat-abliterated-sikaworld-fp4-ltx2/resolve/main/Gemma3-12B-NVFP4-Sikaworld-Pure.safetensors) |
| `Gemma-3-12b HereticX Abliterated` | ![bf16][badge-bf16] | 15 GB | [![][gh-Sikaworld1990]](https://huggingface.co/Sikaworld1990/gemma3-12B-hereticx-sikaworld-ltx-2/resolve/main/gemma3-12B-hereticx-sikaworld.safetensors) |
| `Gemma-3-12b High-Fidelity Abliterated` | ![bf16][badge-bf16] | 14.1 GB | [![][gh-Sikaworld1990]](https://huggingface.co/Sikaworld1990/gemma-3-12b-it-abliterated-sikaworld-high-fidelity-edition-Ltx-2/resolve/main/gemma-3-12b-it-abliterated-sikaworld-high-fidelity-edition.safetensors) |

* FP4-HF: High-fidelity mixed precision calibration
* FP4-Pure: Pure FP4 quantization for maximum compression
* HereticX: Uncensored variant with maximum prompt fidelity
* High-Fidelity: Optimized for quality with better detail preservation

</details>

<p id="enc-heretic" align="center">· · · · · · · · · · · · · ·</p>

### ▣ Gemma-3-12b IT Heretic

Models by [DreamFast](https://huggingface.co/DreamFast). "Heretic" lineage bypasses alignment/restriction layers in the text encoder so LTX-2/2.3 receives the most faithful prompt embeddings. Two upstream versions (v1, v2) plus an AX1Y2JP ultra-uncensored fork and a 3rd-party mradermacher imatrix GGUF re-quant set.

<details>
  <summary>Heretic v1 — DreamFast (bf16 + fp8 + 8 GGUFs)</summary>

#### Safetensors

| Model | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `Gemma_3_12B_it Heretic` | ![bf16][badge-bf16] | 23.5 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic/resolve/main/comfyui/gemma_3_12B_it_heretic.safetensors) |
| `Gemma_3_12B_it Heretic` | ![fp8][badge-fp8] | 12.8 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic/resolve/main/comfyui/gemma_3_12B_it_heretic_fp8_e4m3fn.safetensors) |

#### GGUF

| Quant | Size | Download |
| :---: | :---: | :---: |
| ![F16][badge-F16] | 22 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic/resolve/main/gguf/gemma-3-12b-it-heretic-f16.gguf) |
| ![Q8_0][badge-Q8_0] | 12 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic/resolve/main/gguf/gemma-3-12b-it-heretic-Q8_0.gguf) |
| ![Q6_K][badge-Q6_K] | 9.0 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic/resolve/main/gguf/gemma-3-12b-it-heretic-Q6_K.gguf) |
| ![Q5_K_M][badge-Q5_K_M] | 7.9 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic/resolve/main/gguf/gemma-3-12b-it-heretic-Q5_K_M.gguf) |
| ![Q5_K_S][badge-Q5_K_S] | 7.7 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic/resolve/main/gguf/gemma-3-12b-it-heretic-Q5_K_S.gguf) |
| ![Q4_K_M][badge-Q4_K_M] | 6.8 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic/resolve/main/gguf/gemma-3-12b-it-heretic-Q4_K_M.gguf) |
| ![Q4_K_S][badge-Q4_K_S] | 6.5 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic/resolve/main/gguf/gemma-3-12b-it-heretic-Q4_K_S.gguf) |
| ![Q3_K_M][badge-Q3_K_M] | 5.6 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic/resolve/main/gguf/gemma-3-12b-it-heretic-Q3_K_M.gguf) |

</details>

<details>
  <summary>Heretic v2 — DreamFast (5 safetensors + 8 GGUFs)</summary>

#### Safetensors

| Model | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `gemma-3-12b-it-heretic-v2` | ![bf16][badge-bf16] | 23.25 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic-v2/resolve/main/comfyui/gemma-3-12b-it-heretic-v2.safetensors) |
| `gemma-3-12b-it-heretic-v2` | ![fp8][badge-fp8] | 11.63 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic-v2/resolve/main/comfyui/gemma-3-12b-it-heretic-v2_fp8_e4m3fn.safetensors) |
| `gemma-3-12b-it-heretic-v2` | ![int8tensormixed][badge-int8tensormixed] | 12.60 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic-v2/resolve/main/comfyui/gemma-3-12b-it-heretic-v2_int8.safetensors) |
| `gemma-3-12b-it-heretic-v2` | ![mxfp8mixed][badge-mxfp8mixed] | 12.93 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic-v2/resolve/main/comfyui/gemma-3-12b-it-heretic-v2_mxfp8.safetensors) |
| `gemma-3-12b-it-heretic-v2` | ![nvfp4][badge-nvfp4] | 7.94 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic-v2/resolve/main/comfyui/gemma-3-12b-it-heretic-v2_nvfp4.safetensors) |

#### GGUF

| Quant | Size | Download |
| :---: | :---: | :---: |
| ![F16][badge-F16] | 22.45 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic-v2/resolve/main/gguf/gemma-3-12b-it-heretic-v2-f16.gguf) |
| ![Q8_0][badge-Q8_0] | 11.93 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic-v2/resolve/main/gguf/gemma-3-12b-it-heretic-v2-Q8_0.gguf) |
| ![Q6_K][badge-Q6_K] | 9.21 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic-v2/resolve/main/gguf/gemma-3-12b-it-heretic-v2-Q6_K.gguf) |
| ![Q5_K_M][badge-Q5_K_M] | 8.05 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic-v2/resolve/main/gguf/gemma-3-12b-it-heretic-v2-Q5_K_M.gguf) |
| ![Q5_K_S][badge-Q5_K_S] | 7.85 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic-v2/resolve/main/gguf/gemma-3-12b-it-heretic-v2-Q5_K_S.gguf) |
| ![Q4_K_M][badge-Q4_K_M] | 6.96 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic-v2/resolve/main/gguf/gemma-3-12b-it-heretic-v2-Q4_K_M.gguf) |
| ![Q4_K_S][badge-Q4_K_S] | 6.61 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic-v2/resolve/main/gguf/gemma-3-12b-it-heretic-v2-Q4_K_S.gguf) |
| ![Q3_K_M][badge-Q3_K_M] | 5.73 GB | [![][gh-DreamFast]](https://huggingface.co/DreamFast/gemma-3-12b-it-heretic-v2/resolve/main/gguf/gemma-3-12b-it-heretic-v2-Q3_K_M.gguf) |

</details>

<details>
  <summary>AX1Y2JP Ultra-Uncensored Heretic ComfyUI fp8_scaled</summary>

Ultra-uncensored fork of the Heretic encoder, fp8-scaled and ComfyUI-ready. Single safetensors by [AX1Y2JP](https://huggingface.co/AX1Y2JP).

| Model | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `gemma-3-12b-it-heretic` (ultra-uncensored) | ![fp8][badge-fp8] | 12.99 GB | [![][gh-AX1Y2JP]](https://huggingface.co/AX1Y2JP/Gemma-3-12B-IT-Ultra-Uncensored-Heretic-ComfyUI-fp8/resolve/main/gemma-3-12b-it-heretic-fp8_scaled.safetensors) |

</details>

<details>
  <summary>mradermacher imatrix GGUF re-quant of Heretic v2 (24 quants)</summary>

Third-party imatrix (importance-matrix) re-quantization of DreamFast's Heretic v2 by [mradermacher](https://huggingface.co/mradermacher). Covers the full i1-IQ* and i1-Q*_K* family for low-VRAM use. Sizes verified from the repo file list.

| Quant | Size | Download |
| :---: | :---: | :---: |
| ![IQ1_M][badge-IQ1_M] | 3.02 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-IQ1_M.gguf) |
| ![IQ1_S][badge-IQ1_S] | 2.81 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-IQ1_S.gguf) |
| ![IQ2_M][badge-IQ2_M] | 4.11 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-IQ2_M.gguf) |
| ![IQ2_S][badge-IQ2_S] | 3.83 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-IQ2_S.gguf) |
| ![IQ2_XS][badge-IQ2_XS] | 3.66 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-IQ2_XS.gguf) |
| ![IQ2_XXS][badge-IQ2_XXS] | 3.36 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-IQ2_XXS.gguf) |
| ![IQ3_M][badge-IQ3_M] | 5.39 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-IQ3_M.gguf) |
| ![IQ3_S][badge-IQ3_S] | 5.21 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-IQ3_S.gguf) |
| ![IQ3_XS][badge-IQ3_XS] | 4.96 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-IQ3_XS.gguf) |
| ![IQ3_XXS][badge-IQ3_XXS] | 4.56 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-IQ3_XXS.gguf) |
| ![IQ4_NL][badge-IQ4_NL] | 6.57 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-IQ4_NL.gguf) |
| ![IQ4_XS][badge-IQ4_XS] | 6.25 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-IQ4_XS.gguf) |
| ![Q2_K][badge-Q2_K] | 4.55 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-Q2_K.gguf) |
| ![Q2_K_S][badge-Q2_K_S] | 4.24 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-Q2_K_S.gguf) |
| ![Q3_K_L][badge-Q3_K_L] | 6.18 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-Q3_K_L.gguf) |
| ![Q3_K_M][badge-Q3_K_M] | 5.73 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-Q3_K_M.gguf) |
| ![Q3_K_S][badge-Q3_K_S] | 5.21 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-Q3_K_S.gguf) |
| ![Q4_0][badge-Q4_0] | 6.59 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-Q4_0.gguf) |
| ![Q4_1][badge-Q4_1] | 7.21 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-Q4_1.gguf) |
| ![Q4_K_M][badge-Q4_K_M] | 6.96 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-Q4_K_M.gguf) |
| ![Q4_K_S][badge-Q4_K_S] | 6.61 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-Q4_K_S.gguf) |
| ![Q5_K_M][badge-Q5_K_M] | 8.05 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-Q5_K_M.gguf) |
| ![Q5_K_S][badge-Q5_K_S] | 7.85 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-Q5_K_S.gguf) |
| ![Q6_K][badge-Q6_K] | 9.21 GB | [![][gh-mradermacher]](https://huggingface.co/mradermacher/DreamFast-gemma-3-12b-it-heretic-v2-i1-GGUF/resolve/main/DreamFast-gemma-3-12b-it-heretic-v2.i1-Q6_K.gguf) |

</details>


<p id="split" align="center">◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆</p>

## ▓ Separated Components

Separated LTX2 checkpoint by [Kijai](https://huggingface.co/Kijai/LTXV2_comfy) and [Kijai](https://huggingface.co/Kijai/LTX2.3_comfy) for LTX-2.3. For alternative way to load the models in Comfy.

### ▣ Diffusion Models (Transformer Only)

| Ver | Name | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :---: |
| **2.3** | `ltx-2.3-22b dev` | ![bf16][badge-bf16] | 42 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/ltx-2.3-22b-dev_transformer_only_bf16.safetensors) |
| **2.3** | `ltx-2.3-22b dev`  | ![fp8][badge-fp8] | 23.5 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/ltx-2.3-22b-dev_transformer_only_fp8_scaled.safetensors) |
| **2.3** | `ltx-2.3-22b dev`  | ![mxfp8_block32][badge-mxfp8_block32] | 24.1 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/ltx-2.3-22b-dev_transformer_only_mxfp8_block32.safetensors) |
| **2.3** | `ltx-2.3-22b dev`  | ![fp8_input_scaled][badge-fp8_input_scaled] | 25 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/ltx-2-3-22b-dev_transformer_only_fp8_input_scaled.safetensors) |
| **2.3** | `ltx-2.3-22b distilled` | ![bf16][badge-bf16] | 42 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/ltx-2.3-22b-distilled_transformer_only_bf16.safetensors) |
| **2.3** | `ltx-2.3-22b distilled` | ![fp8_input_scaled][badge-fp8_input_scaled] | 23.5 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/ltx-2.3-22b-distilled_transformer_only_fp8_input_scaled.safetensors) |
| **2.3** | `ltx-2.3-22b distilled v2` | ![fp8_input_scaled v2][badge-fp8_input_scaled]| 23.2 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/ltx-2.3-22b-distilled_transformer_only_fp8_input_scaled_v2.safetensors) |
| **2.3** | `ltx-2.3-22b distilled` | ![fp8][badge-fp8] | 23.5 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/ltx-2.3-22b-distilled_transformer_only_fp8_scaled.safetensors) |
| **2.3** | `ltx-2.3-22b distilled` (experimental) | ![mxfp8][badge-mxfp8_block32] | 24.1 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/experimental/ltx-2.3-22b-distilled_transformer_only_mxfp8_block32.safetensors) |
| **2.3** | `ltx-2.3-22b distilled 1.1` | ![bf16][badge-bf16] | 42 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/ltx-2.3-22b-distilled-1.1_transformer_only_bf16.safetensors) |
| **2.3** | `ltx-2.3-22b distilled 1.1` | ![fp8][badge-fp8] | 25.2 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/ltx-2.3-22b-distilled-1.1_transformer_only_fp8_scaled.safetensors) |
| **2.3** | `ltx-2.3-22b distilled 1.1` (experimental) | ![mxfp8][badge-mxfp8_block32] | 24.1 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/ltx-2.3-22b-distilled-1.1_transformer_only_mxfp8_block32.safetensors) |
| **2.3** | `ltx-2.3-22b dev` | ![int8tensormixed][badge-int8tensormixed] | 20.51 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/ltx-2.3-22b-dev_transformer_only_int8_convrot.safetensors) |
| **2.3** | `ltx-2.3-22b distilled 1.1` | ![int8tensormixed][badge-int8tensormixed] | 20.51 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/ltx-2.3-22b-distilled-1.1_transformer_only_int8_convrot.safetensors) |
| **2.3** | `ltx-2.3-22b distilled v3` | ![fp8_input_scaled][badge-fp8_input_scaled] | 23.86 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/diffusion_models/ltx-2.3-22b-distilled_transformer_only_fp8_input_scaled_v3.safetensors) |
| | | | | |
| **2** | `ltx-2-19b dev` | ![bf16][badge-bf16] | 37.8 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/diffusion_models/ltx-2-19b-dev_transformer_only_bf16.safetensors) |
| **2** | `ltx-2-19b dev` | ![fp8][badge-fp8] | 21.6 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/diffusion_models/ltx-2-19b-dev-fp8_transformer_only.safetensors) |
| **2** | `ltx-2-19b dev` | ![fp4][badge-fp4] | 14.5 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/diffusion_models/ltx-2-19b-dev_fp4_transformer_only.safetensors) |
| **2** | `ltx-2-19b distilled` | ![bf16][badge-bf16] | 37.8 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/diffusion_models/ltx-2-19b-distilled_transformer_only_bf16.safetensors?download=true) |
| **2** | `ltx-2-19b distilled` | ![fp8][badge-fp8] | 21.6 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/diffusion_models/ltx-2-19b-distilled-fp8_transformer_only.safetensors) |

> [!NOTE]  
> input_scaled additionally have activation scaling, and are set to run with fp8 matmuls on supported hardware (roughly 40xx and later Nvidia GPUs).

<a id="components-vae"></a>

### ▣ VAE (Video & Audio)

| Ver | Component | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :--- |
| **2.3** | `Video VAE` | ![BF16][badge-bf16] | 1.45 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/vae/LTX23_video_vae_bf16.safetensors) ┊ [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/vae/ltx-2.3-22b-dev_video_vae.safetensors)|
| **2.3** | `Cinematic Video VAE` | ![BF16][badge-bf16] | 1.38 GB | [![][gh-rzgar]](https://huggingface.co/rzgar/LTX-2.3-Cinematic-VAE/resolve/main/LTX23_video_vae_bf16_cinematic.safetensors) |
| **2.3** | `Audio VAE` | ![BF16][badge-bf16] | 365 MB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/vae/LTX23_audio_vae_bf16.safetensors) ┊ [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/vae/ltx-2.3-22b-dev_audio_vae.safetensors)|
| | | | | |
| **2** | `Video VAE` | ![BF16][badge-bf16] | 2.45 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/VAE/LTX2_video_vae_bf16.safetensors) |
| **2** | `Audio VAE` | ![BF16][badge-bf16] | 218 MB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/VAE/LTX2_audio_vae_bf16.safetensors?download=true) |


<a id="components-embed"></a>

### ▣ Embedding Connectors & Text Projection

| Ver | Name | Precision | Size | Download |
| :--- | :--- | :---: | :---: | :--- |
| **2.3** | `Embeddings Connectors dev` | ![bf16][badge-bf16] | 2.31 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/text_encoders/ltx-2.3_text_projection_bf16.safetensors) ┊ [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/text_encoders/ltx-2.3-22b-dev_embeddings_connectors.safetensors) |
| **2.3** | `Embeddings Connectors distilled` | ![bf16][badge-bf16] | 2.31 GB | [![][gh-Unsloth]](https://huggingface.co/unsloth/LTX-2.3-GGUF/resolve/main/text_encoders/ltx-2.3-22b-distilled_embeddings_connectors.safetensors) |
| | | | | |
| **2** | `Connector dev` | ![bf16][badge-bf16] | 2.86 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/text_encoders/ltx-2-19b-embeddings_connector_dev_bf16.safetensors) |
| **2** | `Connector distilled` | ![bf16][badge-bf16] | 2.86 GB | [![][gh-Kijai]](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/text_encoders/ltx-2-19b-embeddings_connector_distill_bf16.safetensors) |

<p id="lora" align="center">◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆</p>

## ▓ LoRA

### ▣ Enchancer, special

* Lightricks LTX-2.3
  * [LipDub IC-LoRA](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-LipDub) - Enables lip dubbing on top of LTX-2.3 for video dubbing via joint audio-visual diffusion (based on JustDubIt research)
* OmerHagawa
  * [Greenscreen Avatar IC-LoRA](https://huggingface.co/OmerHagawa/ltx2-greenscreen-avatar-ic-lora-vertical-v1) - Greenscreen avatar IC-LoRA for vertical video
* systms
  * [SYSTMS FLW IC-LoRA](https://huggingface.co/systms/SYSTMS-FLW-IC-LORA-LTX-2.3) - Seamless shot-to-shot transitions IC-LoRA with trigger word `FLW`, uses gray frames (RGB 127,127,127) between clips
* [LTX-2.3-IC-LoRA-Colorizer](https://huggingface.co/DoctorDiffusion/LTX-2.3-IC-LoRA-Colorizer) by [DoctorDiffusion](https://huggingface.co/DoctorDiffusion) (331 MB) - Colorize black and white videos
* [JUST-DUB-IT](https://huggingface.co/justdubit/justdubit)
* [Best-Face-Swap-Video](https://huggingface.co/Alissonerdx/BFS-Best-Face-Swap-Video)
* [Image-to-Video Adapter LoRA](https://huggingface.co/MachineDelusions/LTX-2_Image2Video_Adapter_LoRa)
  * Original by MachineDelusions
  * [siraxe variant](https://huggingface.co/siraxe/MachineDelusions_LTX-2_Image2Video_Adapter_LoRa) - Stripped audio layers + rank64 compressed (2.62 GB, 655 MB rank64 bf16)
* Lightricks LTX-2.3
  * [HDR](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-HDR) - Enables 16-bit HDR video generation and converts SDR video to HDR using LogC3 transform for extended dynamic range
  * [Union Control](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Union-Control) - Unified IC-LoRA combining Canny + Depth + Pose control signals for multi-signal video generation conditioning
  * [Motion Track Control](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Motion-Track-Control) - Guides object motion using sparse point trajectories via colored spline overlays on reference videos
* vrgamedevgirl84
  * [Enhancer1](https://huggingface.co/vrgamedevgirl84/LTX2.3_Enhancer1) - Video enhancement LoRA
  * [Enhancer2](https://huggingface.co/vrgamedevgirl84/LTX2.3_enhancer2) - Second video enhancement LoRA
* oumoumad
  * [IC luminance map](https://huggingface.co/oumoumad/ltx-2_IC_LUMIPARTICLES)
  * [LTX-2 IC-LoRA-Ungrade](https://huggingface.co/oumoumad/LTX-2-19b-IC-LoRA-Ungrade) - Removes color grading and contrast from footage, returning neutral ungraded appearance
  * [LTX-2.3 IC-LoRA-Ungrade](https://huggingface.co/oumoumad/LTX-2.3-22b-IC-LoRA-Ungrade) - LTX-2.3 version of color grading removal IC-LoRA
  * [IC-LoRA-Outpaint](https://huggingface.co/oumoumad/LTX-2.3-22b-IC-LoRA-Outpaint) - Extends video canvas by generating new content in black regions (letterbox areas), filling with temporally consistent content
  * [IC-LoRA-ReFocus](https://huggingface.co/oumoumad/LTX-2.3-22b-IC-LoRA-ReFocus) - Removes lens blur and restores focus to out-of-focus footage (lens blur only)
  * [IC-LoRA-Uncompress](https://huggingface.co/oumoumad/LTX-2.3-22b-IC-LoRA-Uncompress) - Removes MP4 compression artifacts (blocking, banding, mosquito noise) and restores clean video
  * [IC-LoRA-MotionDeblur](https://huggingface.co/oumoumad/LTX-2.3-22b-IC-LoRA-MotionDeblur) - Removes motion blur from footage
  * [IC-LoRA-Deinterlace](https://huggingface.co/oumoumad/LTX-2.3-22b-IC-LoRA-Deinterlace) - Removes interlacing artifacts from video
  * [FXIC LTX2 IC-LoRA](https://huggingface.co/oumoumad/fxic-ltx2-iclora) - Flux-inspired IC-LoRA for LTX video transformation with multiple optimizer variants (adamw, prodigy, masked) at various training steps
  * [DeArchive LTX-2.3](https://huggingface.co/oumoumad/ltx-2.3-dearchive-lora) - In-Context LoRA for restoring archive video (old B&W footage, low-res web rips, sepia-toned silent-era prints) into colored, high-definition modern cinematography (Rank 128, 5,000 steps)
* Kijai
  * [Realisdance](https://huggingface.co/Kijai/LTX2-IC-LoRAs/resolve/main/realisdance_ltx2.3_ic-lora_step_02000.safetensors) - IC-LoRA trained on the realisdance dance set (312 MB)
  * [SAM3D Body v42](https://huggingface.co/Kijai/LTX2-IC-LoRAs/resolve/main/ltx23_sam3dbody_v42_restarts-step00004000.comfy.safetensors) - IC-LoRA tied to SAM3D body pose conditioning (624 MB)
* Cseti
  * [IC-LoRA-Cameraman v1](https://huggingface.co/Cseti/LTX2.3-22B_IC-LoRA-Cameraman_v1) - Transfers camera movements (zoom, pan, tilt, orbit) from reference video to generated output
  * [IC-LoRA-EditRefVid v1](https://huggingface.co/Cseti/LTX2.3-22B_IC-LoRA-EditRefVid_v1) - Edit reference video IC-LoRA for editing existing videos using reference guidance
  * [IC-LoRA-Cameraman v2](https://huggingface.co/Cseti/LTX2.3-22B_IC-LoRA-Cameraman_v2) - v2 of the Cameraman IC-LoRA with a larger and more diverse dataset; replicates camera motion from a reference video. No trigger word required.
  * [IC-LoRA-CrossView Prompt v0.9](https://huggingface.co/Cseti/LTX2.3-22B_IC-LoRA-CrossView-Prompt) - Virtual second camera IC-LoRA: give it a reference video + a short camera-angle prompt using the trigger `crossview.` and re-render the same scene from a new viewpoint. v0.9 proof-of-concept trained on synthetic multi-view data; no starting image needed.
  * [IC-LoRA-CrossView Warp v0.9](https://huggingface.co/Cseti/LTX2.3-22B_IC-LoRA-CrossView-Warp) - Depth-warp novel-view IC-LoRA for LTX-Video 2.3 (22B). Given a video + a depth-warp of the same video (from the CrossViewWarp ComfyUI node, Depth Anything V2 input) and an azimuth/elevation/distance offset, renders the scene from that new viewpoint. Sibling of CrossView-Prompt v0.9. (192 MB)

* 100percentrobot
  * [Audio-Reactive LORA](https://huggingface.co/100percentrobot/LTX-2.3-Audio-Reactive-LORA) - Generates audio-reactive videos with motion synchronized to musical elements (beats, rhythm)
* LiconStudio
  * [VBVR-lora-I2V](https://huggingface.co/LiconStudio/Ltx2.3-VBVR-lora-I2V) - Enhances video generation for complex reasoning tasks including multi-object interactions, physical causality, and spatial relationships
  * [VBVR-lora-I2V Special](https://huggingface.co/LiconStudio/Ltx2.3-VBVR-lora-I2V)
  * [Licon MSR V2](https://huggingface.co/LiconStudio/LTX-2.3-Multiple-Subject-Reference) - Multiple Subject Reference v2: IC-LoRA preserving character identity / clothing / objects across frames in multi-reference video generation. Improves consistency, stability and scene logic vs. v1. Requires the [ComfyUI-Licon-MSR](https://github.com/liconstudio/ComfyUI-Licon-MSR) plugin.

* TheBurgstall
  * [LTX-2.3-Skin-Hair](https://huggingface.co/TheBurgstall/LTX-2.3-skin-hair) - Refines skin texture and hair rendering, reduces plastic skin artifacts, improves specular highlights 
  * [VR-360-Outpaint IC-LoRA](https://huggingface.co/TheBurgstall/VR-360-Outpaint-LTX2.3-IC-LoRA) - Outpaints standard widescreen footage into a full 360° equirectangular projection for immersive/VR viewing.
  * [Seamless-Equirectangular LTX-2.3 LoRA](https://huggingface.co/TheBurgstall/Seamless-Equirectangular-LTX2.3-LoRA) - Rank-128 LoRA for equirectangular 360° text-to-video generation with LTX-2.3 (15k steps). Trigger `Equirectangular`. Pairs with the [ComfyUI-Seamless-Equirectangular](https://github.com/Burgstall-labs/ComfyUI-Seamless-Equirectangular) node pack and EquiRoPE / Geometric CFG / per-step roll / circular VAE / wrapped noise setup.

* Nightfury16
  * [Staging IC-lora 512](https://huggingface.co/Nightfury16/ltx2.3-staging-ic-lora-512) - Staging IC-LoRA for video composition control (512 latent scale)
* siraxe
  * [MergeGreen IC-lora](https://huggingface.co/siraxe/MergeGreen_IC-lora_ltx2.3) - Maintains motion at start/end frames, use middle frames with RGB 0,191,0 (75% green fill) in IC-LoRA workflow
  * [TTM IC-lora](https://huggingface.co/siraxe/TTM_IC-lora_ltx2.3) - Makes cutouts cartoony and adds cartoony characters to video scenes, based on the TTM approach (use with Img To Video bypass + Add Video IC-LoRA Guide node)
* Lightricks LTX-2
  * [Canny Control](https://huggingface.co/Lightricks/LTX-2-19b-IC-LoRA-Canny-Control) - Edge detection control for structural guidance
  * [Depth Control](https://huggingface.co/Lightricks/LTX-2-19b-IC-LoRA-Depth-Control) - Depth map conditioning for 3D spatial control
  * [Detailer](https://huggingface.co/Lightricks/LTX-2-19b-IC-LoRA-Detailer) - Enhances fine details and textures in generated videos
  * [Pose Control](https://huggingface.co/Lightricks/LTX-2-19b-IC-LoRA-Pose-Control) - Human pose estimation control for motion guidance

**Upscaler LoRAs:**
* [LTX 2.3 Upscale IC-LoRA](https://huggingface.co/Zlikwid/LTX_2.3_Upscale_IC_Lora) by [Zlikwid](https://huggingface.co/Zlikwid)
  * Generative refinement LoRA for upscaling lower-res or soft videos
  * Works by bicubic upscaling first, then running through LTX 2.3 with this LoRA
  * Use prompt: `upscale`
* [LTX2.3-ICEdit-Insight](https://huggingface.co/joyfox/LTX2.3-ICEdit-Insight) by [JoyFox Lab](https://huggingface.co/joyfox)
  * Task-aware video restoration and editing model family
  * Supports: Video Restoration, HD Enhancement, Watermark Removal, Subtitle Removal
* [Singularity LTX-2.3 OmniCine](https://huggingface.co/WarmBloodAban/Singularity_LTX-2.3_OmniCine_Preview0.1) by [WarmBloodAban](https://huggingface.co/WarmBloodAban)
  * Comprehensive optimizer for LTX2.3 I2V and First/Last Frame workflows
  * Features: Limb Evolution, Shot Injection, Natural Expression, Physical Integrity, Cross-Style Potential
  * Uses "Singularity" prompting framework with 7-block bilingual structure
* yuvraj108c
  * [LTX-2.3-22b-IC-LoRA-Any-Trajectory-Instruction](https://huggingface.co/yuvraj108c/LTX-2.3-22b-IC-LoRA-Any-Trajectory-Instruction) - IC-LoRA porting Any Trajectory Instruction (ATI) to LTX-2.3; lets users draw motion paths on an input image and have the model generate videos following those trajectories (splines). Trained on 25 video pairs at 768x768x81 bucket size, 3000 steps.
* zghhui
  * [OmniNFT RL-LoRA](https://huggingface.co/zghhui/OmniNFT) - Modality-wise Omni Diffusion Negative-aware Fine-Tuning RL-LoRA for joint audio-video generation (paper arXiv:2605.12480). Provides both LTX-2 and LTX-2.3 variants.
  * [LTX-2.3-OmniNFT-RL-LoRA (Kijai mirror)](https://huggingface.co/Kijai/LTX2.3_comfy/resolve/main/loras/LTX-2.3-OmniNFT-RL-Lora_bf16.safetensors) - Same OmniNFT RL-LoRA repackaged by Kijai in bf16 (588 MB).
* VetoBugger
  * [LTX2.3-CrispLora](https://huggingface.co/VetoBugger/LTX2.3-CrispLora) - Crisp enhancement LoRA for LTX-2.3 (`LTX2.3_Crisp_Enhance.safetensors`).
* SyFeee
  * [LTX-2.3 Dual-Character LoRA](https://huggingface.co/SyFeee/LTX2.3-Dual-Character-en) - Image-to-video character-consistency LoRA tuned for two-character dialogue scenes and multi-shot cinematic generation. Works for ancient Chinese fantasy, modern urban, and 3D anime styles. Recommended strength 0.7-0.9 standalone, 0.3-0.5 when stacked with style LoRAs.
* WarmBloodAban
  * [Singularity LTX-2.3 OmniCine V1](https://huggingface.co/WarmBloodAban/Singularity-LTX-2.3_OmniCine_V1) - Updated V1 of the OmniCine integrated optimization framework. Restructures LTX-Video 2.3 generation logic with focus on I2V, First/Last Frame, and Reference-to-Video workflows. Nearly 100,000 training steps. Includes `Singularity-LTX-2.3_OmniCine_V1.safetensors` (2.57 GB) and `Singularity-LTX-2.3_OmniCine_V1nsf.safetensors` (2.57 GB, NSF variant).

<a id="lora-styles"></a>

### ▣ Styles
* OmerHagawa
  * [LTX2 UME PixelArt LoRA](https://huggingface.co/OmerHagawa/ltx2-ume-pixelart-lora) - Pixel art style LoRA for LTX-2
* Playtime-AI
  * [Commission LTX-2.3 MtF Transformation](https://huggingface.co/Playtime-AI/Commission_LTX-2.3-MtF_Transformation_v2.1) - MtF transformation style LoRA for LTX 2.3
* Andro0s
  * [Pixar Toon Style LoRA](https://huggingface.co/Andro0s/LTX_2.3_Pixar_Toon_Style_LoRa) - Pixar-style CGI toon cinematic look with trigger word `P1x4r`
* Cseti
  * [Arcane-Jinx v1](https://huggingface.co/Cseti/LTX2.3-22B_Arcane-Jinx_v1) - Style LoRA inspired by Arcane's Jinx character design
  * [ReStyle IC-LoRA](https://huggingface.co/Cseti/LTX2.3-22B_ReStyle_IC-LoRA) - Image-guided style transfer IC-LoRA that re-renders videos in a target style while preserving original content and motion
* lopho
  * [Gantz O v1.0.0](https://huggingface.co/lopho/ltx2-movie-loras) - Movie-style LoRA (654 MB, 10000 steps)
* bionicman69
  * [Arnold Style](https://huggingface.co/bionicman69/Arnold_LTX23) - Arnold Style LoRA for LTX 2.3. Get to the choppa!
  * [Star Trek TNG Style](https://huggingface.co/bionicman69/StarTrek_TNG_Style_LTX23) - Star Trek: The Next Generation style LoRA for LTX 2.3
* CoachBate
  * [Abercrom-ME](https://huggingface.co/CoachBate/ltx-2.3-22b-ic-lora-abercrom-me) - Vintage A&F Quarterly americana style-transfer IC-LoRA: transforms an input photo (subject + clothing + scene) into moody monochrome / sun-drenched beach / locker-room aesthetics with full styling makeover. Image-conditioned; pairs with the bundled `ABERCROM-ME IC-LoRA by coachbate-v3_20steps_3phase_3stage3.json` workflow. (384 MB, 2000 steps)
* ssjenforcer191
  * [Homelander](https://huggingface.co/ssjenforcer191/Homelander_LTX2.3) - Character IC-LoRA for The Boys' Homelander. Triggerword `HeroHomelander` (optionally append `wearing red leather gloves` / `dark blue cape and ornate red-and-gold collar`). Rank 64, 1500 steps, no regularization. Note: occasional letterbox black bars from training data. (~1.25 GB)
* oumoumad
  * [LTX-2-19b-LoRA-SPROUT](https://huggingface.co/oumoumad/LTX-2-19b-LoRA-SPROUT)
  * [Clay Stop Motion](https://huggingface.co/oumoumad/clay-stop-motion-lora-ngtvspc)
* kabachuha
  * [Hydraulic press](https://huggingface.co/kabachuha/ltx2-hydraulic-press)
  * [Cakeify](https://huggingface.co/kabachuha/ltx2-cakeify)
  * [Big Anime Breasts](https://huggingface.co/kabachuha/ltx2-big-anime-breasts)
  * [Eat](https://huggingface.co/kabachuha/ltx2-eat)
  * [Squish – One Hand Only](https://huggingface.co/kabachuha/ltx2-squish-one-hand)
  * [POP! Inflatable Animation](https://huggingface.co/kabachuha/ltx23-pop) - Comically inflate and pop cartoon/anime characters into confetti and fabric scraps (I2V focused)
* [CRT Animation Terminal](https://huggingface.co/lovis93/crt-animation-terminal-ltx-2.3-lora) by [lovis93](https://huggingface.co/lovis93) - Real late-80s/early-90s CRT monitor look with scanlines, phosphor glow, chromatic aberration, and dithering. Trigger word: `crtanim,`. Available in 4000 and 10000 training steps variants
* vrgamedevgirl84 Style LoRAs
  * [ClayMationStyle](https://huggingface.co/vrgamedevgirl84/LTX2.3_ClayMationStyle) - Clay animation style LoRA for LTX-2.3
  * [Wild West Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Wild_West_Style_LoRa)
  * [Paper Cut Out Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Paper_Cut_Out_Style_LoRa)
  * [Post Apocalyptic Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Post_Apocalyptic_Style_LoRa)
  * [Pixar Toon Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Pixar_Toon_Style_LoRa)
  * [Luxe Sensual Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Luxe_Sensual_Style_LoRa)
  * [Soft Enhance Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Soft_Enhance_Style_LoRa)
  * [Crisp Enhance Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Crisp_Enhance_Style_LoRa)
  * [Fantasy Puppet Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Fantasy_Puppet_Style_LoRa)
  * [Fantasy Realism Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Fantasy_Realism_Style_LoRa)
  * [Fantasy Painterly Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Fantasy_Painterly_Style_LoRa)
  * [Fantasy Anime Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Fantasy_Anime_Style_LoRa)
  * [Cozy Felt Style](https://huggingface.co/vrgamedevgirl84/LTX2.3_Cozy_Felt_Style_LoRa)
  * [Clay Mation Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Clay_Mation_Style_LoRa)
  * [90s Animation Style](https://huggingface.co/vrgamedevgirl84/LTX_2.3_90s_Animation_Style_LoRa)
* [Alissonerdx LTX-LoRAs Collection](https://huggingface.co/Alissonerdx/LTX-LoRAs) - Comprehensive collection including:
  * Anime2Half-Real - Converts anime-style content to half-realistic aesthetic (4500 steps, rank64)
  * Edit-Anything Global - Global editing LoRA variants (6000-9000 steps, rank128)
  * Inpaint Masked R2V/T2V - Region-based inpainting LoRAs for masked video editing
  * Real2Anime/Anime2Real - Style conversion LoRAs (rank64)
* Nebsh
  * [Outfit Switch](https://huggingface.co/Nebsh/LTX2_Outfitswitch)
  * [Handheld run](https://huggingface.co/Nebsh/LTX2_Handheld_run)
  * [Atomic Explosion](https://huggingface.co/Nebsh/LTX2_AtomicExplosion)
  * [HERO CAM](https://huggingface.co/Nebsh/LTX2_Herocam_Lora)
  * [Animatediff V1](https://huggingface.co/Nebsh/LTX2_Animatediff_style)
  * [PUSH TO GLASS](https://huggingface.co/Nebsh/LTX2_Pushtoglass)
  * [Object POV](https://huggingface.co/Nebsh/POVObject)
* [Squish](https://huggingface.co/ovi054/LTX-2-19b-Squish-LoRA)
* [Yoshiaki Kawajiri Retro Anime](https://huggingface.co/tarn59/Yoshiaki_Kawajiri_Retro_Anime_LTX2) - LoRA trained on Yoshiaki Kawajiri's distinctive retro anime art style
* Playtime-AI
  * [DonaldTrump](https://huggingface.co/Playtime-AI/LTX-2.DonaldTrump)
  * [Rick_and_Morty](https://huggingface.co/Playtime-AI/LTX-2.3-Rick_and_Morty-BETA) - BETA LoRA for Rick and Morty animated style
  * [LTX-2.3-Rick_And_Morty_v2](https://huggingface.co/Playtime-AI/LTX-2.3-Rick_And_Morty_v2) - Updated Rick and Morty v2 LoRA trained on the Smith and Rick Sanchez characters (undertrained; voices/clothing can be off; v3 in training)
  * [LTX-2.3-Wednesday_Addams](https://huggingface.co/Playtime-AI/LTX-2.3-Wednesday_Addams)
  * [LTX-2.3-Kermit_the_Frog](https://huggingface.co/Playtime-AI/LTX-2.3-Kermit_the_Frog)
  * [LTX-2.3-Jenna_Coleman](https://huggingface.co/Playtime-AI/LTX-2.3-Jenna_Coleman)
  * [LTX-2.3-Marge_Simpson](https://huggingface.co/Playtime-AI/LTX-2.3-Marge_Simpson) - Marge Simpson character LoRA trained on the base LTX-2.3 Dev model. Trigger words: `2d animation`, `Marge Simpson` (use `2d animation` to avoid getting 3D animation)
  * [LTX-2.3-Bender](https://huggingface.co/Playtime-AI/LTX-2.3-Bender) - Bender (Futurama) character LoRA. Trigger words: `2d animation`, `Bender the bending robot`
  * [LTX-2.3 Sulphur Gyrating Hips](https://huggingface.co/Playtime-AI/LTX-2.3_Sulphur-Gyrating_Hips) - Motion LoRA driven by the trigger `She thrusts her hips in a sexual manner`
* SOLRICKS
  * [LTX-2.3-Yesilcam-Turkish-Cinema](https://huggingface.co/SOLRICKS/LTX-2.3-Yesilcam-Turkish-Cinema) - Nostalgic Yeşilçam Turkish cinema visual style with warm cinematic tones and classic film atmosphere. Recommended strength 0.7.
  * [ltx-2-3-ue5-style-lora](https://huggingface.co/SOLRICKS/ltx-2-3-ue5-style-lora) - Unreal Engine 5 (UE5) cinematic style LoRA. Trigger word: `ue5_style`.
  * [Sci-Fi Cinema](https://huggingface.co/SOLRICKS/ltx-2.3-sci-fi-cinema) - a cinematic science-fiction style LoRA for LTXV / LTX-2.3. Trigger word: `srx_scifilm`.
  * [LTX-2.3 Product Ad Style](https://huggingface.co/SOLRICKS/ltx-2.3-product-ad-style) - Cinematic product-commercial style for luxury / cosmetics / tech / fashion ads. Trigger `srx_commercial`, recommended strength 0.85.
  * [LTX-2.3 The Art of Marbling](https://huggingface.co/SOLRICKS/ltx-2.3-the-art-of-marbling) - Marbling / ebru ink-flow style (paper, pigment, fluid art, Turkish ebru). Trigger `srx_ebrumotion`, recommended strength 0.85.
* SyFeee Chinese Drama Pack
  * [ltx2.3-chinese-drama-charlora](https://huggingface.co/SyFeee/ltx2.3-chinese-drama-charlora) - Character LoRA trained on 78 episodes of Chinese historical drama; specialises base model for live-action, photoreal cinematic generation in Han dynasty / wuxia settings. Trigger words: `char_0_person` through `char_9_person`. Recommended strength 0.8–0.9.
  * [ltx2.3-chinese-drama-iclora-canny](https://huggingface.co/SyFeee/ltx2.3-chinese-drama-iclora-canny) - IC-LoRA conditioning on Canny edge/line-art video; controls scene composition and architectural layout from reference outlines. Use with `char_0_person` for character reference.
  * [ltx2.3-chinese-drama-iclora-depth](https://huggingface.co/SyFeee/ltx2.3-chinese-drama-iclora-depth) - IC-LoRA conditioning on monocular depth video (Depth-Anything-3); transfers 3D geometric structure from reference to generated video. Strong on interior scenes.
  * [ltx2.3-chinese-drama-iclora-pose](https://huggingface.co/SyFeee/ltx2.3-chinese-drama-iclora-pose) - IC-LoRA conditioning on DWPose 133-keypoint skeleton render; transfers pose from reference video while preserving Chinese drama style. Stackable with character LoRA.
* mxturbo
  * [Formula1-Cockpit-T-Cam-LTX2.3](https://huggingface.co/mxturbo/Formula1-Cockpit-T-Cam-LTX2.3) - LoRA trained on 1.6L V6 Turbo Hybrid Era F1 T-Cam onboard footage. Generates cockpit/T-cam onboard video. Trigger: `16LV6HybridF1` (car type); follow the "T-cam onboard view..." / "AT-cam onboard view..." prompt style.
* chsengni
  * [ltx2.3-fpv-motion](https://huggingface.co/chsengni/ltx2.3-fpv-motion) - Smoother FPV (First Person View) camera movements and improved low-speed flight shots.
* EllaPriest45
  * [LTX2.3-characters](https://huggingface.co/EllaPriest45/LTX2.3-characters) - Massive collection of 70+ per-character LoRAs (Abigail Spencer, Adam Driver, Alexandra Daddario, Ana de Armas, Anne Hathaway, Brad Pitt, Cate Blanchett, Chris Evans, Emma Stone, Emma Watson, Eva Green, Gal Gadot, etc.) for LTX-2.3 (Apache 2.0). Each `Name - LTX2.3.safetensors` ~327 MB.
* TheBurgstall
  * [LTX-2.3-Body-Positivity](https://huggingface.co/TheBurgstall/ltx-2.3-bodypositivity-lora)
  * [LTX-2.3-Googly-Eyes](https://huggingface.co/TheBurgstall/ltx-2.3-googlyeyes-lora)
* TheBurgstall (LTX-2)
  * [EarthZoomOut](https://huggingface.co/TheBurgstall/EarthZoomOut-LoRA-LTX-2-19b)
  * [GroupPhoto](https://huggingface.co/TheBurgstall/GroupPhoto-LoRA-LTX-2-19b)
  * [WHATUSEE](https://huggingface.co/TheBurgstall/WHATUSEE_LTX-2-19B_LoRA)
* [Black Venom](https://huggingface.co/siraxe/black_venom_ltx2)
* Lightricks
  * [Camera Control: dolly-in](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Dolly-In/blob/main/ltx-2-19b-lora-camera-control-dolly-in.safetensors)
  * [Camera Control: dolly-left](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Dolly-Left/blob/main/ltx-2-19b-lora-camera-control-dolly-left.safetensors)
  * [Camera Control: dolly-out](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Dolly-Out/blob/main/ltx-2-19b-lora-camera-control-dolly-out.safetensors)
  * [Camera Control: dolly-right](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Dolly-Right/blob/main/ltx-2-19b-lora-camera-control-dolly-right.safetensors)
  * [Camera Control: jib-down](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Jib-Down/blob/main/ltx-2-19b-lora-camera-control-jib-down.safetensors)
  * [Camera Control: jib-up](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Jib-Up/blob/main/ltx-2-19b-lora-camera-control-jib-up.safetensors)
  * [Camera Control: static](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Static/blob/main/ltx-2-19b-lora-camera-control-static.safetensors)
  * [Union-Control](https://huggingface.co/Lightricks/LTX-2-19b-IC-LoRA-Union-Control/resolve/main/ltx-2-19b-ic-lora-union-control-ref0.5.safetensors)
* eraRelentless
  * [LTXreal](https://huggingface.co/eraRelentless/ltx23REALISM) - Realism stylization for LTX-2.3; trigger `realism`
* nnndite
  * [ltx2.3 Foot Model](https://huggingface.co/nnndite/ltx2.3foot) - Foot / lower-limb LoRA for LTX-2.3
* fal
  * [LTX-2.3 IC-LoRA — 3D Render to Photoreal](https://huggingface.co/fal/LTX-2.3-3DREAL-LoRA) - IC-LoRA turning rough 3D viewport / Blender blockouts into photoreal cinematic video while preserving composition and camera. Trigger `3DREAL`. v2 (`3DREAL-strong-v2`) is the newest and is also exposed on fal.ai as `render-to-real`.
* a3xrfgb
  * [Fable 5 — Vintage Style LoRA](https://huggingface.co/a3xrfgb/Fable5_Ltx2.3_vintage_style) - Vintage-style minimal-illustration / stop-motion / typography LoRA for LTX-2.3, used in the Fable 5 intro. Trained on a personal RTX 3090 (~5 hours).

<a id="lora-special"></a>

### ▣ Special

* [Wan2.1 VAE Adapter](https://huggingface.co/HDHCDev/Ltx2_2_Wan2.1_VAE_Adapter)
  * Latent space adapter for converting between LTX-2 and Wan2.1 VAE representations
  * `latent_adapter_final.pt` (447 MB)
* TenStrip
  * [LTX2.3 JoyAI LoRA Extracted](https://huggingface.co/TenStrip/LTX2.3_JoyAI_Lora_Extracted) - LoRA extracted from [jdopensource/JoyAI-Echo](https://huggingface.co/jdopensource/JoyAI-Echo); boosts prompt response and motion in LTX-2.3 (also used for NSFW/Sulphur/Eros) at strength 0.4–0.7.
  * [LTX2.3 DMD LoRA](https://huggingface.co/TenStrip/LTX2.3_DMD_Lora) - DMD-distillation delta extraction in [JoyAI-Echo](https://huggingface.co/jdopensource/JoyAI-Echo), reshaped for LTX-2.3 384-rank 1.1 sampling. Sample sigmas in the card.
* ltx-community
  * [ltx2-compile-keytest](https://huggingface.co/ltx-community/ltx2-compile-keytest) - IC-LoRA fine-tune from `ltx-2.3-22b-dev.safetensors` (300 training steps, batch size 1, LR 2e-4). Trained with the [LTX LoRA Trainer](https://huggingface.co/spaces/ltx-community/ltx2-lora-trainer).
* Lightricks
  * [LTX-2.3-22b-LoRA-Foley-V2A](https://huggingface.co/Lightricks/LTX-2.3-22b-LoRA-Foley-V2A) - Official Lightricks Foley V2A (video-to-audio) LoRA for LTX-2.3. Generates realistic, visually-synced Foley sound effects from video. Rank ~small (216 MB); pairs with the workflow JSON in the repo (`ltx-2.3-foley-v2a.json`).
  * [LTX-2.3-22b-IC-LoRA-Clean-Plate](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Clean-Plate) - Official Lightricks Clean-Plate IC-LoRA. Removes people/objects from video frames for steady background plates. Rank 128 (312 MB); pairs with the `LTX-2.3_-_V2V_mass_remove_people_Clean-Plate-Lora.json` workflow.
  * [LTX-2.3-22b-IC-LoRA-Relight](https://huggingface.co/Lightricks/LTX-2.3-22b-IC-LoRA-Relight/resolve/main/ltx-2.3-22b-ic-lora-relight-1.0.safetensors) - Official Lightricks Relight IC-LoRA (single-stage, distilled). Relights a scene using a reference sphere image that defines the target lighting direction and color. Pairs with the bundled `LTX-2.3_Relight_ICLoRA_SingleStage_Distilled.json` workflow. (312 MB)
* fbjr
  * [LTX-2.3-22b-IC-LoRA-Audio-Only-Context](https://huggingface.co/fbjr/LTX-2.3-22b-IC-LoRA-Audio-Only-Context) - Two IC-LoRA checkpoints for audio-only and cross-modal audio-video context conditioning on LTX-2.3. Audio-only checkpoint (156 MB, `audio_only_step_01000.safetensors`) preserves a reference audio identity through a generation pass; cross-modal checkpoint (276 MB, `cross_modal_step_01000.safetensors`) extends that to joint audio-video conditioning.
* FuzzPuppy
  * [LTX-2.3 Foley](https://huggingface.co/FuzzPuppy/LTX-2.3-Foley-LoRA) - Video-to-audio LoRA for LTX-2.3 that adds realistic, visually synchronized Foley / sound effects over a video (multiplier 1.0–3.0; pairs with the LTX Community License).
* Hoffm4nz
  * [LTX-2.3-22b-IC-LoRA-Golden-Hour](https://huggingface.co/Hoffm4nz/LTX-2.3-22b-IC-LoRA-Golden-Hour) - IC-LoRA fine-tune that biases generation toward warm "Golden Hour" lighting aesthetics. Root canonical checkpoint `ltx-2.3-22b-ic-lora-golden-hour.safetensors` (312 MB); four per-step snapshots are also available in the `checkpoints/` folder of the repo (step_00250 → step_01000, 312 MB each).

* vpakarinen
  * [Motion Stabilizer for LTX-2.3](https://huggingface.co/vpakarinen/motion-stabilizer-ltx-23) - Motion LoRA stabilises body movement and rotation in LTX-2.3.
* Comfy-Org
  * [ltx-2.3-22b-ic-lora-ingredients-0.9](https://huggingface.co/Comfy-Org/ltx-2.3/resolve/main/split_files/loras/ltx-2.3-22b-ic-lora-ingredients-0.9.safetensors) - Comfy-Org-distributed ingredients IC-LoRA for LTX-2.3 (the other three siblings in the same folder — `id-lora-celebvhq-3k`, `id-lora-talkvid-3k`, `distilled_1.1_lora_dynamic_fro09_avg_rank_111_bf16` — are already linked from the Checkpoints / ID-LoRA tables).
* linoyts
  * [ltx2.3-ic-lora-ingredients-multishot](https://huggingface.co/linoyts/ltx2.3-ic-lora-ingredients-multishot) - IC-LoRA fine-tune from `ltx-2.3-22b-dev.safetensors` (2,500 training steps, LR 1e-4). Trained for multi-shot ingredient-conditioned generation.
  * [ltx2-ic-lora-ui](https://huggingface.co/linoyts/ltx2-ic-lora-ui) - LoRA fine-tune from `ltx-2.3-22b-dev.safetensors` (20 training steps; treats UI-screen aesthetics). Inherits LTX-2.3 base license.
* rzgar
  * [Motion Enhancer (N54W)](https://huggingface.co/rzgar/LTX-2.3-Motion-Enhancer-n4w/resolve/main/LTX-2.3-Motion-Enhancer-n4w.safetensors) - General-purpose N54W motion enhancer LoRA. Enhances fluidity, coherence, and motion when stacked as a companion LoRA alongside other specialized models. Extensively tested with top-rated Civitai LoRAs. (2.17 GB)


<a id="lora-id-lora"></a>

### ▣ ID-LoRA (Identity-Driven In-Context LoRA)

**ID-LoRA** is a method that enables identity-preserving audio-video generation in a single model. It jointly generates a subject's appearance and voice, letting a text prompt, a reference image, and a short audio clip govern both modalities together. Built on top of LTX-2.3 (22B), it is the **first method to personalize visual appearance and voice within a single generative pass**.

Unlike cascaded pipelines that treat audio and video separately, ID-LoRA operates in a **unified latent space** where a single text prompt can simultaneously dictate the scene's visual content, environmental acoustics, and speaking style—while preserving the subject's vocal identity and visual likeness.

**Key Features:**
- Text prompt controls the scene and content
- Reference image preserves the subject's visual likeness
- Short audio clip preserves the subject's vocal identity
- Single unified generation pass for both appearance and voice

**Available LoRAs for LTX-2.3:**

| LoRA | LoRA Rank | Size | Download |
|:---|:---|:---:|:---|
| ID-LoRA-TalkVid-3K | 128 | 1.1 GB | [![][gh-AviadDahan]](https://huggingface.co/AviadDahan/LTX-2.3-ID-LoRA-TalkVid-3K) ┊ [![][gh-Comfy--Org]](https://huggingface.co/Comfy-Org/ltx-2.3/resolve/main/split_files/loras/ltx-2.3-id-lora-talkvid-3k.safetensors) |
| ID-LoRA-CelebVHQ-3K | 128 | 1.1 GB | [![][gh-AviadDahan]](https://huggingface.co/AviadDahan/LTX-2.3-ID-LoRA-CelebVHQ-3K) ┊ [![][gh-Comfy--Org]](https://huggingface.co/Comfy-Org/ltx-2.3/resolve/main/split_files/loras/ltx-2.3-id-lora-celebvhq-3k.safetensors) |

**Resources:**
- [Project Page](https://id-lora.github.io/) | [GitHub](https://github.com/ID-LoRA/ID-LoRA) | [Paper (arXiv: 2603.10256)](https://arxiv.org/abs/2603.10256)

<p id="nodes" align="center">◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆</p>

## ▓ ComfyUI Nodes

### ▣ Custom Node Collections

* [10S-Comfy-nodes](https://github.com/TenStrip/10S-Comfy-nodes) by TenStrip - Custom ComfyUI nodes for improving motion quality when working with LTX 2.3's combined audio/video latent pipeline. Includes Latent Cross Fade Auto Concat, Audio Latent Stretch, Latent Motion Sharpener, Latent Temporal Upsampler, Latent Motion Retime, and Latent Temporal Inpainter for clean 30fps output from 24fps sampled models.

* [Deno Custom Nodes](https://github.com/Deno2026/comfyui-deno-custom-nodes) by Deno2026 - Practical ComfyUI custom nodes focused on fast real-world workflow improvements including (Deno) Resize Box, Multi Image Loader, LTX Sequencer, LTX Model Loader, Easy Model Download Helper, LTX Multi LoRA Loader, and LTX Prompt Guide.

* [PromptRelay](https://github.com/kijai/ComfyUI-PromptRelay) by kijai - Enables consistent multilingual lip-sync while maintaining voice consistency across languages. Distributes video latent frames across segments with smart prompt node supporting inline and block syntax styles.

* [WhatDreamsCost ComfyUI](https://github.com/WhatDreamsCost/WhatDreamsCost-ComfyUI) by WhatDreamsCost - LTX Director 2.0 plus a variety of custom ComfyUI nodes and workflows for creating AI-generated video content including Multi Image Loader, LTX Sequencer, LTX Keyframer, Speech Length Calculator, Load Video UI, and Load Audio UI. 1.7k+ stars.

* [ComfyUI-Sapiens2](https://github.com/kijai/ComfyUI-Sapiens2) by kijai - ComfyUI nodes for Sapiens2 computer vision models from Facebook Research. Supports pose estimation, body-part segmentation, surface normal estimation, and pointmap estimation with model variants from 400M to 5B parameters.


<p id="training" align="center">◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆</p>

## ▓ LoRA Training

For training **LTX LoRAs**, the community uses a variety of official scripts, community-developed forks, and cloud-based platforms.

### Primary Local Training Tools

* **Official LTX-2 Trainer:** This is the standard Python-based package for training LoRAs, full fine-tuning, and In-Context (IC) LoRAs. It is designed for Linux and requires CUDA and Triton.
    * **Link:** [Official LTX-2 Trainer Repository](https://github.com/Lightricks/LTX-2/tree/main/packages/ltx-trainer)
* **Musubi-Tuner (AkaneTendo25 Fork):** Widely considered the **fastest and most efficient** local trainer for LTX-2 and 2.3. It features significantly smaller cache sizes (up to 12x smaller than AI Toolkit) and better iteration speeds, reaching up to **2 iterations per second on an RTX 5090**.
    * **Link:** [AkaneTendo25 Musubi-Tuner Fork](https://github.com/AkaneTendo25/musubi-tuner)
* **AI Toolkit (by Ostris):** A popular third-party tool that supports LTX-2 character and image-to-video LoRAs. While beginner-friendly, some users reported issues with audio training on the main branch.
    * **Link:** [Official AI Toolkit Repository](https://github.com/ostris/ai-toolkit)
* **AI Toolkit: BIG-DADDY-VERSION (ArtDesignAwesome Fork):** This specific fork was created to **fix broken audio and voice training** in the original AI Toolkit. It is optimized for hardware like the RTX 5090.
    * **Link:** [ArtDesignAwesome AI Toolkit Fork](https://github.com/ArtDesignAwesome/ai-toolkit_BIG-DADDY-VERSION)
* **rs-nodes (richservo):** A collection of nodes that includes a **full LTX Lora trainer directly within ComfyUI**. It is designed to be memory-efficient, allowing training on cards with as little as **11GB-12GB of VRAM** by using ComfyUI's native weight loaders.
    * **Link:** [rs-nodes ComfyUI Trainer](https://github.com/richservo/rs-nodes)
* **SimpleTuner:** A highly optimized trainer for Linux that supports LTX-2 and is noted for its ability to handle larger datasets on limited VRAM via block swapping.
    * **Link:** [SimpleTuner Repository](https://github.com/bghira/SimpleTuner)

<a id="training-cloud"></a>

### Cloud Training Platforms

* **Fal.ai:** Provides a dedicated cloud trainer for custom styles and effects, though it is primarily limited to image-based training datasets.
    * **Link:** [Fal.ai LTX2 Video Trainer](https://fal.ai/models/fal-ai/ltx2-video-trainer)
* **RunComfy:** A cloud service that offers a pre-configured AI Toolkit setup specifically for LTX-2 training.
    * **Link:** [RunComfy LTX-2 Training](https://www.runcomfy.com/trainer/ai-toolkit/ltx-2-lora-training)

<a id="training-dataset"></a>

### Essential Dataset & Captioning Tools

* **Taz's Ultimate Captioning Tool:** A Hugging Face space frequently used by the community to generate the **long, detailed, cinematographic prompts** (around 200 words) that LTX-2 requires for high-quality training.
    * **Link:** [LoRA Caption Assistant (Hugging Face)](https://huggingface.co/spaces/comfyuiman/loracaptionertaz_v2)
* **AI Video Clipper & LoRA Captioner:** A modular pipeline designed to automate local dataset creation using WhisperX and Qwen2-VL, including support for RTX 5090 Blackwell cards.
    * **Link:** [AI Video Clipper & LoRA Captioner](https://github.com/cyberbol/AI-Video-Clipper-LoRA)

<a id="training-requirements"></a>

### Training Requirements Summary

* **Dataset:** Videos should typically be cut to **121 frames** (exactly 4.84 seconds) to align with the model's architectural "8n+1" rule.
* **Hardware:** While 16GB VRAM is possible with extreme offloading in tools like **rs-nodes**, **24GB is the practical minimum** for quantized training. For best results and speed, **48GB to 80GB (H100 or RTX 6000)** is preferred.
* **Precision:** It is now officially recommended to train on the **full BF16 model** for LTX 2.3 rather than FP8 for superior quality.


<p id="wf" align="center">◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆</p>

## ▓  Workflow & Technical Notes

### ❖ RuneXX

**[RuneXX](https://huggingface.co/RuneXX/LTX-2.3-Workflows) LTX-2.3 Workflows:**


* [I2V T2V Basic](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/LTX-2.3_-_I2V_T2V_Basic.json)
* [I2V T2V Basic GGUF](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/LTX-2.3_-_I2V_T2V_Basic_GGUF.json)
* [I2V T2V Dev Full-Steps](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/LTX-2.3_-_I2V_T2V_Dev_Full-Steps.json)
* [I2V T2V Simple Single Pass](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/LTX-2.3_-_I2V_T2V_Simple_single_pass.json)
* [T2V Basic](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/LTX-2.3_-_T2V_Basic.json)
* [T2V Simple Single Pass](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/LTX-2.3_-_T2V_Simple_single_pass.json)

**Movie-Maker:**

* [I2V Short-Story PromptRelay-Timeline multi-image multi-sequence](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Movie-Maker/LTX-2.3_-_I2V_Short-Story_PromptRelay-Timeline_multi-image_multi-sequence.json)
* [I2V Short-Story PromptRelay multi-image multi-sequence](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Movie-Maker/LTX-2.3_-_I2V_Short-Story_PromptRelay_multi-image_multi-sequence.json)
* [I2V T2V Short-Story PromptRelay-Timeline multi-sequence](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Movie-Maker/LTX-2.3_-_I2V_T2V_Short-Story_PromptRelay-Timeline_multi-sequence.json)
* [I2V T2V Short-Story PromptRelay multi-sequence](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Movie-Maker/LTX-2.3_-_I2V_T2V_Short-Story_PromptRelay_multi-sequence.json)

**Multi-ref-character-sheet:**

* [I2V Multi-subject Reference Licon-MSR V1-lora (older version)](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Multi-ref-character-sheet/Older-Version/LTX-2.3_-_I2V_multi-subject-reference_Licon-MSR-V1-lora_older_version.json)
* [I2V Multi-subject Reference Licon-MSR V2 LTX-Ingredients OmniNTF Experimental](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Multi-ref-character-sheet/LTX-2.3_-_I2V_multi-subject-reference_Licon-MSR-V2-LTX-Ingredients-OmniNTF_Experimental.json)
* [I2V Multi-subject Reference Licon-MSR V2-lora](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Multi-ref-character-sheet/LTX-2.3_-_I2V_multi-subject-reference_Licon-MSR-V2-lora.json)
* [T2V/R2V Character Sheet Best-Face-ID LoRA](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Multi-ref-character-sheet/LTX-2.3_-_T2V_R2V_character-sheet_Best-Face-ID-Lora.json)
* [T2V/R2V Face-ref + audio-ref Best-Face-ID LoRA + ID-LoRA audio](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Multi-ref-character-sheet/LTX-2.3_-_T2V_R2V_face-ref-audio-ref_Best-Face-ID-Lora-ID-Lora_audio.json)
* [T2V/R2V Face-ref + custom audio Best-Face-ID LoRA](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Multi-ref-character-sheet/LTX-2.3_-_T2V_R2V_face-ref-custom-audio_Best-Face-ID-Lora.json)
* [T2V/R2V Face-ref image only Best-Face-ID LoRA](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Multi-ref-character-sheet/LTX-2.3_-_T2V_R2V_face-ref-image_Best-Face-ID-Lora.json)

**Helper-wf:**

* [Flux-Klein Character Sheet from ref image](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Multi-ref-character-sheet/Helper-wf/Flux_Klein_-_Character_Sheet_from_ref_image.json)
* [Ideogram Reference Sheet for Ingredients LoRA](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Multi-ref-character-sheet/Helper-wf/Ideogram_-_Reference_Sheet_for_Ingredients_lora.json)
* [Qwen-Image Character Sheet from ref image ZIT refiner](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Multi-ref-character-sheet/Helper-wf/Qwen_Image_-_Character_Sheet_from_ref_image_ZIT_refiner.json)

**Talking-Avatar-TTS:**

* [I2V T2V Talking Avatar (Qwen-TTS)](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Talking-Avatar-TTS/LTX-2.3_-_I2V_T2V_Talking_Avatar_(voice_clone_with_Qwen-TTS).json)
* [I2V T2V Talking Avatar (Fish-Audio-Pro)](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Talking-Avatar-TTS/LTX-2.3_-_I2V_T2V_Talking_Avatar_(voice_clone_with_Fish-Audio-Pro).json)
* [I2V T2V Talking Avatar (OmniVoice-TTS)](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Talking-Avatar-TTS/LTX-2.3_-_I2V_T2V_Talking_Avatar_(voice_clone_with_OmniVoice-TTS).json)

**Video-2-Video:**

*Just-Talk — add voice to silent video:*
* [V2V Just Talk Prompt Lip-synced Voice](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/Just-Talk_add_voice_to_silent_video/LTX-2.3_-_V2V_Just_Talk_prompt_lip-synced-voice_to_any_video.json)
* [V2V Just Talk Prompt Lipsynced Voice Sam3](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/Just-Talk_add_voice_to_silent_video/LTX-2.3_-_V2V_Just_Talk_prompt_lipsynced-voice_to_any_video_Sam3.json)
* [V2V Just Talk Custom Audio Lip-synced To Any Video](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/Just-Talk_add_voice_to_silent_video/LTX-2.3_-_V2V_Just_Talk_custom_audio_lip-synced_to_any_video.json)
* [V2V Just Talk Dub Any Silent Video Multilanguage](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/Just-Talk_add_voice_to_silent_video/LTX-2.3_-_V2V_Just_Talk_dub_any_silent_video_multilanguage.json)

*Extend-Any-Video:*
* [V2V Extend Any Video](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/Extend-Any-Video/LTX-2.3_-_V2V_Extend_Any_Video.json)
* [V2V Extend Any Video Multi-Extend Long Video](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/Extend-Any-Video/LTX-2.3_-_V2V_Extend_Any_Video_Multi-Extend_long_video.json)
* [V2V Extend Any Video towards Last-Frame-image](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/Extend-Any-Video/LTX-2.3_-_V2V_Extend_Any_Video_towards_Last-Frame-image.json)

*Inpaint:*
* [V2V Inpainting Inpaint-T2V-lora Sam3-Masking](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/Inpaint/LTX-2.3_-_V2V_inpainting_Inpaint-T2V-lora_Sam3-Masking.json)
* [V2V Inpainting Inpaint-T2V-lora Sam2-Point-Masking](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/Inpaint/LTX-2.3_-_V2V_inpainting_Inpaint-T2V-lora_Sam2-Point-Masking.json)

*Shot-to-Shot-Transition:*
* [V2V Shot-to-Shot Transition Systms-FLW-lora](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/Shot-to-Shot-Transition/LTX-2.3_-_V2V_shot-to-shot-transition_Systms-FLW-lora.json)
* [V2V Shot-to-Shot Transition MergeGreen IC-Lora](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/Shot-to-Shot-Transition/LTX-2.3_-_V2V_shot-to-shot-transition_MergeGreen-IC-Lora.json)
* [V2V Shot-to-Shot Transition Re-Take Inpaint](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/Shot-to-Shot-Transition/LTX-2.3_-_V2V_shot-to-shot-transition_Re-Take_inpaint.json)

*Other:*
* [V2V Remove Watermark Subtitles ICEdit-Insight-lora](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/LTX-2.3_-_V2V_remove_watermark_subtitles_ICEdit-Insight-lora.json)
* [V2V Expand Any Video IC-Lora-Outpaint](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/LTX-2.3_-_V2V_Expand_Any_Video_IC-Lora-Outpaint.json)
* [V2V Foley Add Sound To Any Video (Foley-Lora)](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/LTX-2.3_-_V2V_Foley_Add_Sound_To_Any_Video_Foley-Lora.json)
* [V2V ReTake recreate any section of any video](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/LTX-2.3_-_V2V_ReTake_recreate_any_section_of_any_video.json)
* [V2V Video-Edit remove add replace restyle EditAnything-Lora](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/LTX-2.3_-_V2V_Video-Edit_remove_add_replace_restyle_EditAnything-Lora.json)
* [V2V High Dynamic Range IC-HDR-lora](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/LTX-2.3_-_V2V_high_dynamic_range_IC-HDR-lora.json)
* [V2V Just-Dub-It Multilanguage Dubbing IC-Lora-LipDub](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/LTX-2.3_-_V2V_Just-Dub-It_multilanguage_dubbing_IC-Lora-LipDub.json)
* [V2V Change Viewpoint Angle CrossView-Lora](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/LTX-2.3_-_V2V_Change_viewpoint_angle_CrossView-Lora.json)
* [V2V Upscale Any Video Pixel-Spatial-Lora](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/LTX-2.3_-_V2V_Upscale-Any-Video-Pixel-Spatial-Lora.json)
* [V2V Mass Remove People Clean-Plate-Lora](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Video-2-Video/LTX-2.3_-_V2V_mass_remove_people_Clean-Plate-Lora.json)

**Music-Video-Creator:****Music-Video-Creator:**
* [I2V T2V Music-Video multi-scene full render](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Music-Video-Creator/LTX-2.3_-_I2V_T2V_Music-Video_multi-scene_full_render.json)
* [I2V T2V Music-Video multi-scene save per segment](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Music-Video-Creator/LTX-2.3_-_I2V_T2V_Music-Video_multi-scene_save_per_segment.json)
* [I2V T2V Music-Video Prompt-Relay multi-scene save per segment](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Music-Video-Creator/LTX-2.3_-_I2V_T2V_Music-Video_Prompt-Relay_multi-scene_save_per_segment.json)
  * **Helper-Workflows:**
    * [AceStep-XL create music from a prompt](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Music-Video-Creator/Helper-Workflows/AceStep-XL_create_music_from_a_prompt.json)
    * [Flux-Klein transform firstframe](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Music-Video-Creator/Helper-Workflows/Flux-Klein_transform_firstframe.json)
    * [Qwen-Image transform firstframe next scene or different angle LoRA](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Music-Video-Creator/Helper-Workflows/Qwen-Image_transform_firstframe_next_scene_or_different_angle_lora.json)
    * [Video merge combine with interpolate upscale](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Music-Video-Creator/Helper-Workflows/Video_merge_combine_with_interpolate_upscale.json)

**Others:**
* [I2V T2V Basic custom audio with Gemma-API example](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Others/LTX-2.3_-_I2V_T2V_Basic_custom_audio_with_Gemma-API_example.json)

**Custom-Audio:**

* [I2V T2V Basic ID-Lora Reference Audio](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Custom-Audio/LTX-2.3_-_I2V_T2V_Basic_ID-Lora_reference_audio.json) 
* [I2V T2V Dev Custom Audio](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Custom-Audio/LTX-2.3_-_I2V_T2V_Dev_Custom_Audio.json) 
* [I2V T2V Basic Custom Audio](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Custom-Audio/LTX-2.3_-_I2V_T2V_Basic_Custom_Audio.json) 

**First-Last-Frame:**
* [First-Last-Frame Workflows](https://huggingface.co/RuneXX/LTX-2.3-Workflows/tree/main/First-Last-Frame)
* [FLF2V First Last Frame](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/First-Last-Frame/LTX-2.3_-_FLF2V_First-Last-Frame.json)
* [FLF2V First Last Frame Custom Audio](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/First-Last-Frame/LTX-2.3_-_FLF2V_First-Last-Frame_custom_audio.json)
* [FLF2V First Last Frame Transition LoRA](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/First-Last-Frame/LTX-2.3_-_FLF2V_First-Last-Frame_transition_lora.json)
* [FML2V First Middle Last Frame Guider](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/First-Last-Frame/LTX-2.3_-_FML2V_First_Middle_Last_Frame_Guider.json)
* [FML2V First Middle Last Frame Injection](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/First-Last-Frame/LTX-2.3_-_FML2V_First_Middle_Last_Frame_Injection.json)
* [FML2V Guider Custom Audio](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/First-Last-Frame/LTX-2.3_-_FML2V_Guider_Custom_Audio.json)

**Long-Video-Experimental:**

* [I2V T2V Long Video Custom Audio Loop](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Long-Video-Experimental/LTX-2.3_-_I2V_T2V_Long_Video_Custom_Audio_Loop.json)
* [I2V T2V Long Video Custom Audio](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Long-Video-Experimental/LTX-2.3_-_I2V_T2V_Long_Video_Custom_Audio.json)
* [I2V T2V Long Video Custom Audio singlepass loop](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Long-Video-Experimental/LTX-2.3_-_I2V_T2V_Long_Video_Custom_Audio_singlepass_loop.json)

**3-Pass-Experimental:**

* [I2V T2V Experimental 3-pass 1.5x Upscaler](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/3-Pass-Experimental/LTX-2.3_-_I2V_T2V_Experimental_3-Pass.json)
* [I2V T2V DEV Experimental 3-Pass](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/3-Pass-Experimental/LTX-2.3_-_I2V_T2V_DEV_Experimental_3-Pass.json)

**Control-reference:**

* [I2V TV2V Transfer Camera Movements IC-Cameraman LoRA](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Control-reference/LTX-2.3_-_IV2V_TV2V_transfer_camera_movements_IC-Cameraman_lora.json)
* [I2V TV2V Transfer Body Movements IC-Union-Control-lora DWPose](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Control-reference/LTX-2.3_-_IV2V_TV2V_transfer_body_movements_IC-Union-Control-lora_DWPose.json)
* [I2V TV2V Transfer Body Movements IC-Union-Control-lora SDPose](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Control-reference/LTX-2.3_-_IV2V_TV2V_transfer_body_movements_IC-Union-Control-lora_SDPose.json)
* [I2V TV2V Transfer Body Movements IC-RealisDance-lora](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Control-reference/LTX-2.3_-_IV2V_TV2V_transfer_body_movements_IC-RealisDance-lora.json)


**Helper-Workflows:**

* [AceStep-XL Create Music From a Prompt](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Music-Video-Creator/Helper-Workflows/AceStep-XL_create_music_from_a_prompt.json)
* [Flux-Klein Transform Firstframe](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Music-Video-Creator/Helper-Workflows/Flux-Klein_transform_firstframe.json)
* [Qwen-Image Transform Firstframe Next Scene or Different Angle LoRA](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Music-Video-Creator/Helper-Workflows/Qwen-Image_transform_firstframe_next_scene_or_different_angle_lora.json)

**Other-examples:**

* [I2V T2V Basic Custom Audio with Gemma-API](https://huggingface.co/RuneXX/LTX-2.3-Workflows/resolve/main/Other-examples/LTX-2.3_-_I2V_T2V_Basic_custom_audio_with_Gemma-API_example.json)

<details>
  <summary>RuneXX LTX-2 Workflows old pre_feb2026</summary>

* [First Last Frame (guide node)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20First%20Last%20Frame%20(guide%20node).json)
* [First Last Frame (in-place node)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20First%20Last%20Frame%20(in-place%20node).json)
* [First Middle Last Frame (guide node)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20First%20Middle%20Last%20Frame%20(guide%20node).json)
* [I2V Basic (GGUF)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20I2V%20Basic%20(GGUF).json)
* [I2V Basic](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20I2V%20Basic.json)
* [I2V IC-Control (pose)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20I2V%20IC-Control%20(pose).json)
* [I2V Simple First Middle Last Frame (1-pass K-Sampler)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20I2V%20Simple%20First%20Middle%20Last%20Frame%20(1-pass%20K-Sampler).json)
* [I2V Talking Avatar (voice clone Qwen-TTS)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20I2V%20Talking%20Avatar%20(voice%20clone%20Qwen-TTS).json)
* [I2V and T2V (beta test sampler previews)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20I2V%20and%20T2V%20(beta%20test%20sampler%20previews).json)
* [I2V and T2V Basic (Custom Audio)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20I2V%20and%20T2V%20Basic%20(Custom%20Audio).json)
* [I2V and T2V IC-Control (All-In-One Pose Canny Depth)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20I2V%20and%20T2V%20IC-Control%20(All-In-One%20Pose%20Canny%20Depth).json)
* [I2V and T2V Simple (1-pass K-Sampler)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20I2V%20and%20T2V%20Simple%20(1-pass%20K-Sampler).json)
* [I2V and T2V Simple (1-pass)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20I2V%20and%20T2V%20Simple%20(1-pass).json)
* [T2V Basic (GGUF)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20T2V%20Basic%20(GGUF).json)
* [T2V Basic (low vram)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20T2V%20Basic%20(low%20vram).json)
* [T2V Basic](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20T2V%20Basic.json)
* [T2V Talking Avatar (voice clone Qwen-TTS)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20T2V%20Talking%20Avatar%20(voice%20clone%20Qwen-TTS).json)
* [V2A Foley (add sound to any video)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20V2A%20Foley%20(add%20sound%20to%20any%20video).json)
* [V2V (extend any video)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20V2V%20(extend%20any%20video).json)
* [V2V Head Swap Experimental (BFS lora)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20V2V%20Head%20Swap%20Experimental%20(BFS%20lora).json)
* [V2V Just Dub It (experimental)(translate speech auto dubbing)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20V2V%20Just%20Dub%20It%20(experimental)(translate%20speech%20auto%20dubbing).json)
* [V2V Just Dub It (with voice clone)(auto dubbing translation)(experimental)](https://huggingface.co/RuneXX/LTX-2-Workflows/resolve/main/older_comfy_pre_feb2026/LTX-2%20-%20V2V%20Just%20Dub%20It%20(with%20voice%20clone)(auto%20dubbing%20translation)(experimental).json)
</details>

<p align="center">═══●═══●═══●═══●═══●═══●═══●═══●═══</p>

<a id="wf-lightricks"></a>

### ❖ Lightricks

**[LTX-2.3](https://github.com/Lightricks/ComfyUI-LTXVideo/tree/master/example_workflows/2.3)**:
* [ICLoRA Motion Track Control](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/2.3/LTX-2.3_ICLoRA_Motion_Track_Distilled.json)
* [Union Control](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/2.3/LTX-2.3_ICLoRA_Union_Control_Distilled.json)
* [Single Stage](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/2.3/LTX-2.3_T2V_I2V_Single_Stage_Distilled_Full.json)
* [Two Stage](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/2.3/LTX-2.3_T2V_I2V_Two_Stage_Distilled.json)

**[LTX-2](https://github.com/Lightricks/ComfyUI-LTXVideo/tree/master/example_workflows/2.0)**:
* [Text to Video Full](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/2.0/LTX-2_T2V_Full_wLora.json)
* [Text to Video Distilled](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/2.0/LTX-2_T2V_Distilled_wLora.json)
* [Image to Video Full](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/2.0/LTX-2_I2V_Full_wLora.json)
* [Image to Video Distilled](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/2.0/LTX-2_I2V_Distilled_wLora.json)
* [ICLoRA](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/2.0/LTX-2_ICLoRA_All_Distilled.json)
* [Video to Video](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/2.0/ltx-2-v2v.json)
* [Video to Video Detailer](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/2.0/LTX-2_V2V_Detailer.json)

<a id="wf-vrgamedevgirl84"></a>

### ❖ vrgamedevgirl84

**[vrgamedevgirl84](https://huggingface.co/vrgamedevgirl84) LTX 2.3 Music Video Creator:**

* [Music Video Creator Workflow](https://huggingface.co/vrgamedevgirl84/LTX_2.3_Music_Video_Creator_ComfyUI)
  * Prompt Creator Workflow - Audio upload, beat detection, scene timing, lyrics analysis, style selection, prompt generation
  * Text-to-Video Workflow - LoRA integration, advanced prompt controls, Remake Mode, video stitching
  * Image-to-Video Workflow - Uses Z-Image Turbo and LTX 2.3
  * Requirements: ComfyUI, LTX 2.3 models, Z-Image Turbo model, FFmpeg, vrgamedevgirl custom nodes
  
<a id="wf-comfyui"></a>

### ❖ ComfyUI

* [Text-to-video](https://raw.githubusercontent.com/Comfy-Org/workflow_templates/refs/heads/main/templates/video_ltx2_t2v.json)
* [Text-to-video Distilled (faster, 8 steps)](https://raw.githubusercontent.com/Comfy-Org/workflow_templates/refs/heads/main/templates/video_ltx2_t2v_distilled.json)
* [Image-to-video](https://raw.githubusercontent.com/Comfy-Org/workflow_templates/refs/heads/main/templates/video_ltx2_t2v_distilled.json)
* [Image-to-video Distilled (faster, 8 steps)](https://raw.githubusercontent.com/Comfy-Org/workflow_templates/refs/heads/main/templates/video_ltx2_i2v_distilled.json)
* [Depth control](https://github.com/Comfy-Org/workflow_templates/raw/refs/heads/main/templates/video_ltx2_depth_to_video.json)
* [Canny control](https://raw.githubusercontent.com/Comfy-Org/workflow_templates/refs/heads/main/templates/video_ltx2_canny_to_video.json)
* [Pose control](https://raw.githubusercontent.com/Comfy-Org/workflow_templates/refs/heads/main/templates/video_ltx2_pose_to_video.json)


<!-- MARKDOWN LINKS & IMAGES -->
[stars-shield]: https://img.shields.io/github/stars/wildminder/awesome-ltx2.svg?style=for-the-badge
[stars-url]: https://github.com/wildminder/awesome-ltx2/stargazers
[telegram-shield]: https://img.shields.io/badge/TokenDiff-26A5E4?style=for-the-badge&logo=telegram&logoColor=white
[telegram-url]: https://t.me/TokenDiff
[x-shield]: https://img.shields.io/badge/wildmindai-000000?style=for-the-badge&logo=x&logoColor=white
[x-url]: https://x.com/wildmindai

[gh-Abiray]: https://img.shields.io/badge/Abiray-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-joeygambino]: https://img.shields.io/badge/joeygambino-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-Hoffm4nz]: https://img.shields.io/badge/Hoffm4nz-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[badge-int4mixedtensorwise]: https://img.shields.io/badge/int4mixedtensor-17a2b8?style=flat-square

[badge-IQ1_M]: https://img.shields.io/badge/IQ1__M-e05d44?style=flat-square
[badge-IQ1_S]: https://img.shields.io/badge/IQ1__S-e05d44?style=flat-square
[badge-IQ2_M]: https://img.shields.io/badge/IQ2__M-e05d44?style=flat-square
[badge-IQ2_S]: https://img.shields.io/badge/IQ2__S-e05d44?style=flat-square
[badge-IQ2_XS]: https://img.shields.io/badge/IQ2__XS-e05d44?style=flat-square
[badge-IQ2_XXS]: https://img.shields.io/badge/IQ2__XXS-e05d44?style=flat-square
[badge-IQ3_M]: https://img.shields.io/badge/IQ3__M-fe7d37?style=flat-square
[badge-IQ3_S]: https://img.shields.io/badge/IQ3__S-fe7d37?style=flat-square
[badge-IQ3_XS]: https://img.shields.io/badge/IQ3__XS-fe7d37?style=flat-square
[badge-IQ3_XXS]: https://img.shields.io/badge/IQ3__XXS-fe7d37?style=flat-square
[badge-IQ4_NL]: https://img.shields.io/badge/IQ4__NL-dfb317?style=flat-square
[badge-IQ4_XS]: https://img.shields.io/badge/IQ4__XS-dfb317?style=flat-square
[gh-AX1Y2JP]: https://img.shields.io/badge/AX1Y2JP-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-AviadDahan]: https://img.shields.io/badge/AviadDahan-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-Comfy--Org]: https://img.shields.io/badge/Comfy--Org-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-DaSiWa]: https://img.shields.io/badge/DaSiWa-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-DreamFast]: https://img.shields.io/badge/DreamFast-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-FusionCow]: https://img.shields.io/badge/FusionCow-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-fbjr]: https://img.shields.io/badge/fbjr-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-Kijai]: https://img.shields.io/badge/Kijai-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-Lightricks]: https://img.shields.io/badge/Lightricks-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-mradermacher]: https://img.shields.io/badge/mradermacher-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-QuantStack]: https://img.shields.io/badge/QuantStack-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-SexGod1979]: https://img.shields.io/badge/SexGod1979-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-Sikaworld1990]: https://img.shields.io/badge/Sikaworld1990-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-SOLRICKS]: https://img.shields.io/badge/SOLRICKS-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-SulphurAI]: https://img.shields.io/badge/Sulphur_2_base-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-TenStrip]: https://img.shields.io/badge/TenStrip-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-TheStageAI]: https://img.shields.io/badge/TheStageAI-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-Unsloth]: https://img.shields.io/badge/Unsloth-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-Winnougan]: https://img.shields.io/badge/Winnougan-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-drbaph]: https://img.shields.io/badge/drbaph-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-silveroxides]: https://img.shields.io/badge/silveroxides-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-vantagewithai]: https://img.shields.io/badge/vantagewithai-lightgrey?style=flat-square&logo=huggingface&logoColor=white

[badge-BF16]: https://img.shields.io/badge/BF16-0077cc?style=flat-square
[badge-F16]: https://img.shields.io/badge/F16-0077cc?style=flat-square
[badge-Q2_K]: https://img.shields.io/badge/Q2__K-e05d44?style=flat-square
[badge-Q2_K_S]: https://img.shields.io/badge/Q2__K__S-e05d44?style=flat-square
[badge-Q3_K_M]: https://img.shields.io/badge/Q3__K__M-fe7d37?style=flat-square
[badge-Q3_K_S]: https://img.shields.io/badge/Q3__K__S-fe7d37?style=flat-square
[badge-Q3_K_L]: https://img.shields.io/badge/Q3__K__L-fe7d37?style=flat-square
[badge-Q4_0]: https://img.shields.io/badge/Q4__0-dfb317?style=flat-square
[badge-Q4_1]: https://img.shields.io/badge/Q4__1-dfb317?style=flat-square
[badge-Q4_K_M]: https://img.shields.io/badge/Q4__K__M-dfb317?style=flat-square
[badge-Q4_K_S]: https://img.shields.io/badge/Q4__K__S-dfb317?style=flat-square
[badge-Q5_0]: https://img.shields.io/badge/Q5__0-97c00f?style=flat-square
[badge-Q5_1]: https://img.shields.io/badge/Q5__1-97c00f?style=flat-square
[badge-Q5_K_M]: https://img.shields.io/badge/Q5__K__M-97c00f?style=flat-square
[badge-Q5_K_S]: https://img.shields.io/badge/Q5__K__S-97c00f?style=flat-square
[badge-Q6_K]: https://img.shields.io/badge/Q6__K-0077cc?style=flat-square
[badge-Q8_0]: https://img.shields.io/badge/Q8__0-28a745?style=flat-square
[badge-UD-Q2_K]: https://img.shields.io/badge/UD-Q2__K-e05d44?style=flat-square
[badge-UD-Q3_K_M]: https://img.shields.io/badge/UD-Q3__K__M-fe7d37?style=flat-square
[badge-UD-Q4_K_M]: https://img.shields.io/badge/UD-Q4__K__M-dfb317?style=flat-square
[badge-UD-Q4_K_S]: https://img.shields.io/badge/UD-Q4__K__S-dfb317?style=flat-square
[badge-UD-Q5_K_M]: https://img.shields.io/badge/UD-Q5__K__M-97c00f?style=flat-square
[badge-bf16]: https://img.shields.io/badge/bf16-0077cc?style=flat-square
[badge-fp4]: https://img.shields.io/badge/fp4-ffc107?style=flat-square
[badge-fp8]: https://img.shields.io/badge/fp8-28a745?style=flat-square
[badge-fp8_input_scaled]: https://img.shields.io/badge/fp8__input__scaled-fe7d37?style=flat-square
[badge-int8mixedtensorwise]: https://img.shields.io/badge/int8mixedtensorwise-17a2b8?style=flat-square
[badge-int8tensormixed]: https://img.shields.io/badge/int8tensormixed-17a2b8?style=flat-square
[badge-mxfp8_block32]: https://img.shields.io/badge/mxfp8__block32-20c997?style=flat-square
[badge-mxfp8mixed]: https://img.shields.io/badge/mxfp8mixed-20c997?style=flat-square
[badge-nvfp4]: https://img.shields.io/badge/nvfp4-6f42c1?style=flat-square
[gh-BingoG]: https://img.shields.io/badge/BingoG-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-CoachBate]: https://img.shields.io/badge/CoachBate-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-Cseti]: https://img.shields.io/badge/Cseti-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-ssjenforcer191]: https://img.shields.io/badge/ssjenforcer191-lightgrey?style=flat-square&logo=huggingface&logoColor=white
[gh-rzgar]: https://img.shields.io/badge/rzgar-lightgrey?style=flat-square&logo=huggingface&logoColor=white
