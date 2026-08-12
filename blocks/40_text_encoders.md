<p id="text-encoder" align="center">◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆</p>

## ▓ Text Encoders

LTX-2/2.3 require Gemma-3-12b variants with text projection layers. **LTX-2.5 ships with a Gemma-4-12B** text encoder — see the ▣ Gemma-4-12b section below.

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

<a id="enc-gemma4"></a>

### ▣ Gemma-4-12b (LTX-2.5 Text Encoders)

LTX-2.5 replaces the Gemma-3-12B text encoder with a **Gemma-4-12B** encoder. Community "heretic" / uncensored forks bypass alignment layers for maximum prompt fidelity in downstream video generation.

| Model | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `gemma4-12b-heretic-ltx-2.5` | ![bf16][badge-bf16] | 24.46 GB | [![][gh-ibyteohdear]](https://huggingface.co/ibyteohdear/gemma4-12b-heretic-ltx-2.5-bf16/resolve/main/gemma4-12b-heretic-ltx-2.5-bf16.safetensors) |
| `Gemma-4-12B-it-uncensored-heretic` | ![int8convrot](https://img.shields.io/badge/int8_ConvRot-17a2b8?style=flat-square) | 12.26 GB | [![][gh-DeepNeuralNerd]](https://huggingface.co/DeepNeuralNerd/Gemma-4-12B-it-uncensored-heretic-DeepNeuralNerd-LTX_2.5_ComfyUI/resolve/main/Gemma-4-12B-it-uncensored-heretic%20-%20DeepNeuralNerd%20-LTX%202.5-ComfyUI-int8convrot.safetensors) |
| `gemma4-12b-ltx2.5-int4int8-mix` | ![int4int8mix](https://img.shields.io/badge/int4_int8_mix-17a2b8?style=flat-square) | 7.52 GB | [![][gh-Abiray]](https://huggingface.co/Abiray/LTX-2.5-Gemma4-12B-int4-int8mix-TextEncoder/resolve/main/gemma4-12b-ltx2.5-int4int8-mix.safetensors) |

