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
| **2.5** | `dev` | ![bf16][badge-bf16] | 39.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5/resolve/main/diffusion_models/ltx-2.5-22b-dev-transformer-bf16.safetensors) |
| **2.5** | `dev` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 20.0 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5/resolve/main/diffusion_models/ltx-2.5-22b-dev-transformer-comfy-int8-convrot.safetensors) |
| **2.5** | `distilled` | ![bf16][badge-bf16] | 39.1 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5/resolve/main/diffusion_models/ltx-2.5-22b-distilled-transformer-bf16.safetensors) |
| **2.5** | `distilled` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 20.0 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5/resolve/main/diffusion_models/ltx-2.5-22b-distilled-transformer-comfy-int8-convrot.safetensors) |
| **2.5** | `distilled` | ![nvfp4][badge-nvfp4] | 17.4 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5/resolve/main/diffusion_models/ltx-2.5-22b-distilled-transformer-nvfp4.safetensors) |
| **2.5** | `pt` (pre-trained) | ![bf16][badge-bf16] | 43.0 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5-Pre-Trained/resolve/main/ltx-2.5-22b-pt-bf16.safetensors) |
| **2.5** | `distilled` | ![nvfp4][badge-nvfp4] | 20.6 GB | [![][gh-rockerBOO]](https://huggingface.co/rockerBOO/ltx-2.5-nvfp4-convrot/resolve/main/ltx-2.5-22b-distilled-transformer_nvfp4_convrot_int8.safetensors) |
| **2.5** | `distilled` | ![w4a8](https://img.shields.io/badge/w4a8-17a2b8?style=flat-square) | 11.7 GB | [![][gh-Winnougan]](https://huggingface.co/Winnougan/ltx-2.5-w4a8-convrot-int4-convrot-Winnougan-Blessing/resolve/main/diffusion_models/ltx-2.5-22b-distilled-transformer-w4a8_convrot.safetensors) |
| **2.5** | `distilled` | ![fp8][badge-fp8] | 19.6 GB | [![][gh-vonkaiser]](https://huggingface.co/vonkaiser/LTX-2.5-FP8-NVFP4/resolve/main/transformer/ltx-2.5-22b-distilled-fp8.safetensors) |
| **2.5** | `distilled` | ![nvfp4][badge-nvfp4] | 17.4 GB | [![][gh-BennyDaBall]](https://huggingface.co/BennyDaBall/LTX-2.5-22b-distilled-nvfp4-comfy/resolve/main/ltx-2.5-22b-distilled-transformer-nvfp4-comfy.safetensors) |
| **2.5** | `dev` | ![w4a8](https://img.shields.io/badge/w4a8-17a2b8?style=flat-square) | 14.4 GB | [![][gh-tsolful]](https://huggingface.co/tsolful/LTX_2.5_INT4_W4A8_ConvRot/resolve/main/ltx-2.5-22b-dev-transformer_W4A8_Mixed.safetensors) |
| **2.5** | `distilled` | ![w4a8](https://img.shields.io/badge/w4a8-17a2b8?style=flat-square) | 14.4 GB | [![][gh-tsolful]](https://huggingface.co/tsolful/LTX_2.5_INT4_W4A8_ConvRot/resolve/main/ltx-2.5-22b-distilled-transformer_W4A8_Mixed.safetensors) |
| **2.5** | `distilled` | ![fp8][badge-fp8] | 21.9 GB | [![][gh-guillaume127]](https://huggingface.co/guillaume127/LTX-2.5-FP8/resolve/main/ltx-2.5-22b-distilled-transformer-fp8_e4m3fn.safetensors) |
| | | | | |
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
| **2.3** | `ltx23_srx fp8_e4m3 experimental` | ![fp8][badge-fp8] | 23.1 GB | [![][gh-SOLRICKS]](https://huggingface.co/SOLRICKS/ltx23_srx_fp8_e4m3_experimental/resolve/main/ltx23_srx_fp8_e4m3_experimental.safetensors) |
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
| **2.5** | `spatial-upscaler x2 1.0` | 0.93 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5/resolve/main/latent_upscale_models/ltx-2.5-latent-spatial-upscaler-x2-bf16-1.0.safetensors) ┊ [![][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.5-turbo-GGUF/resolve/main/split/latent_upscale_models/ltx-2.5-latent-spatial-upscaler-x2-bf16-1.0.safetensors) |
| **2.3** | `spatial-upscaler x2 1.0` | 996 MB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-spatial-upscaler-x2-1.0.safetensors) |
| **2.3** | `spatial-upscaler x1.5 1.0` | 1.09 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.3/resolve/main/ltx-2.3-spatial-upscaler-x1.5-1.0.safetensors) |
| | | | |
| **2** | `spatial-upscaler x2 1.0` | 1.05 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-spatial-upscaler-x2-1.0.safetensors) |


<p id="ckpt-temporal-upscaler" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ Temporal Upscaler

Required for current two-stage pipeline implementations in this repository. Download to `COMFYUI_ROOT_FOLDER/models/latent_upscale_models` folder.

| Ver | Name | Size | Download |
| :--- | :--- | :--- | :--- |
| **2.5** | `temporal-upscaler x2 1.0` | 0.24 GB | [![][gh-Lightricks]](https://huggingface.co/Lightricks/LTX-2.5/resolve/main/latent_upscale_models/ltx-2.5-latent-temporal-upscaler-x2-bf16-1.0.safetensors) ┊ [![][gh-ChrisColeTech]](https://huggingface.co/ChrisColeTech/LTX-2.5-turbo-GGUF/resolve/main/split/latent_upscale_models/ltx-2.5-latent-temporal-upscaler-x2-bf16-1.0.safetensors) |
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
| **2.3** | Full | `10Eros v1 INT8 ConvRot` | ![int8](https://img.shields.io/badge/int8-17a2b8?style=flat-square) | 23.51 GB | [![bertbobson][gh-bertbobson]](https://huggingface.co/bertbobson/LTX2.3-10Eros-INT8-ConvRot/resolve/main/10Eros_v1_bf16-int8.ConvRot.safetensors) |

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

<p id="finetune-spatialav2av" align="center">· · · · · · · · · · · · · ·</p>

#### ❖ SpatialAV2AV (BingoG)

Publicly-released audio→audio-video training checkpoints from [BingoG/LTX-2-SpatialAV2AV-Checkpoints](https://huggingface.co/BingoG/LTX-2-SpatialAV2AV-Checkpoints) for spatial-audio conditioned video generation. Two curriculum layouts (`E4` Core Dual + Dynamic; `E6` reserved for Full) at 480p cap, 113 frames at 25 fps.

| Curriculum | Step | Size | Download |
| :--- | :---: | :---: | :---: |
| E4 Core (Dual + Dynamic) | 400  | 36.22 GB | [![BingoG][gh-BingoG]](https://huggingface.co/BingoG/LTX-2-SpatialAV2AV-Checkpoints/resolve/main/E4/step_00400/model_weights_step_00400.safetensors) |
| E4 Core (Dual + Dynamic) | 1000 | 36.22 GB | [![BingoG][gh-BingoG]](https://huggingface.co/BingoG/LTX-2-SpatialAV2AV-Checkpoints/resolve/main/E4/step_01000/model_weights_step_01000.safetensors) |
| E6 Full                  | 1000 | 36.22 GB | [![BingoG][gh-BingoG]](https://huggingface.co/BingoG/LTX-2-SpatialAV2AV-Checkpoints/resolve/main/E6/step_01000/model_weights_step_01000.safetensors) |

*Note: these are intermediate training checkpoints, not inference-ready models — useful for fine-tuning experiments and reproducibility only.*
