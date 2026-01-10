# Awesome LTX-2

A curated list of models, text encoders, and tools for the LTX-2 video generation suite.

## Models

LTX-2 models are available in various formats including full weights, transformers-only, and GGUF quantizations for efficient inference.

### Checkpoints
* **[Lightricks/LTX-2](https://huggingface.co/Lightricks/LTX-2)** - Official repository.

| Name | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `dev` | bf16 | 43.3 GB | [Link](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-dev.safetensors)
| `dev` | fp8 | 27.1 GB | [Link](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-dev-fp8.safetensors)
| `dev` | fp4 | 20 GB | [Link](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-dev-fp4.safetensors)
| `distilled` | bf16 | 43.3 GB | [Link](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-distilled.safetensors)
| `distilled` | fp8 | 27.1 GB | [Link](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-distilled-fp8.safetensors)
  
### GGUF Quantized Models
These models are optimized for lower memory usage. Note that in ComfyUI, these are typically loaded as transformer-only models.

#### **Unsloth GGUFs**
| File Name | Size | Download |
| :--- | :--- | :--- |
| `ltx-2-19b-dev-BF16.gguf` | 37.8 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-BF16.gguf?download=true) |
| `ltx-2-19b-dev-Q8_0.gguf` | 20.4 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q8_0.gguf?download=true) |
| `ltx-2-19b-dev-Q6_K.gguf` | 16.0 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q6_K.gguf?download=true) |
| `ltx-2-19b-dev-Q4_K_M.gguf` | 12.8 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q4_K_M.gguf?download=true) |
| `ltx-2-19b-dev-Q4_0.gguf` | 11.3 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q4_0.gguf?download=true) |

#### **Vantage AI GGUFs (Dev)**
| File Name | Size | Download |
| :--- | :--- | :--- |
| `ltx-2-19b-dev-Q8_0.gguf` | 20.4 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q8_0.gguf?download=true) |
| `ltx-2-19b-dev-Q6_K.gguf` | 15.9 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q6_K.gguf?download=true) |
| `ltx-2-19b-dev-Q4_K_M.gguf` | 12.8 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q4_K_M.gguf?download=true) |

*   **Other GGUF Sources:** [QuantStack/LTX-2-GGUF](https://huggingface.co/QuantStack/LTX-2-GGUF)

### Distilled LoRA

| Rank | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `384` | bf16 | 7.67 GB | [Link](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-distilled-lora-384.safetensors)
| `242` | bf16 | 4.88 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/loras/ltx-2-19b-distilled-lora-resized_dynamic_fro095_avg_rank_242_bf16.safetensors) |
| `175` | bf16 | 3.58 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/loras/ltx-2-19b-distilled-lora_resized_dynamic_fro09_avg_rank_175_bf16.safetensors) |
| `175` | fp8 | 1.79 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/loras/ltx-2-19b-distilled-lora_resized_dynamic_fro09_avg_rank_175_fp8.safetensors) |

---

## Text Encoders

LTX-2 requires Gemma-3-12b variants.

### **Comfy-Org Optimized Encoders**
Official and optimized versions for ComfyUI.

| Model Name | Note | Size | Download |
| :--- | :--- | :---: | :---: |
| `gemma_3_12B_it.safetensors` |  | 24.4 GB | [Link](https://huggingface.co/Comfy-Org/ltx-2/resolve/main/split_files/text_encoders/gemma_3_12B_it.safetensors?download=true) |
| `gemma_3_12B_it_fpmixed.safetensors` | Experimental quant. Should be better than the fp8 scaled | 13.7 GB | [Link](https://huggingface.co/Comfy-Org/ltx-2/resolve/main/split_files/text_encoders/gemma_3_12B_it_fpmixed.safetensors?download=true) |
| `gemma_3_12B_it_fp8_scaled.safetensors` |  | 13.2 GB | [Link](https://huggingface.co/Comfy-Org/ltx-2/resolve/main/split_files/text_encoders/gemma_3_12B_it_fp8_scaled.safetensors?download=true) |
| `gemma_3_12B_it_fp4_mixed.safetensors` | 90% fp4 layers | 9.5 GB | [Link](https://huggingface.co/Comfy-Org/ltx-2/resolve/main/split_files/text_encoders/gemma_3_12B_it_fp4_mixed.safetensors?download=true) |


### **Gemma-3-12b Abliterated**
Fixed versions of the abliterated Gemma-3-12b-it model by [FusionCow](https://huggingface.co/FusionCow/Gemma-3-12b-Abliterated-LTX2), modified specifically for compatibility with LTX-2. The [original model](https://huggingface.co/mlabonne/gemma-3-12b-it-abliterated-v2)

| Model | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `Gemma ablit fixed` | bf16 | 23.5 GB | [Link](https://huggingface.co/FusionCow/Gemma-3-12b-Abliterated-LTX2/resolve/main/gemma_ablit_fixed_bf16.safetensors?download=true) |
| `Gemma ablit fixed` | fp8 | 13.8 GB | [Link](https://huggingface.co/FusionCow/Gemma-3-12b-Abliterated-LTX2/resolve/main/gemma_ablit_fixed_fp8.safetensors?download=true) |

---

## Separated Components

Separated LTX2 checkpoint by [Kijai](https://huggingface.co/Kijai/LTXV2_comfy). For alternative way to load the models in Comfy

### Diffusion Models (Transformer Only)

| Name | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `dev` | bf16 | 37.8 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/diffusion_models/ltx-2-19b-dev_transformer_only_bf16.safetensors)
| `dev` | fp8 | 21.6 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/diffusion_models/ltx-2-19b-dev-fp8_transformer_only.safetensors)
| `distilled` | fp8 | 21.6 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/diffusion_models/ltx-2-19b-distilled-fp8_transformer_only.safetensors)



### VAE (Video & Audio)
| Component | Precision | Size | Download Link |
| :--- | :---: | :---: | :---: |
| **Video VAE** | BF16 | 2.49 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/VAE/LTX2_video_vae_bf16.safetensors?download=true) |
| **Audio VAE** | BF16 | 218 MB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/VAE/LTX2_audio_vae_bf16.safetensors?download=true) |

### Embedding Connectors

| Name | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `Connector dev` | bf16 | 2.86 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/text_encoders/ltx-2-19b-embeddings_connector_dev_bf16.safetensors)
| `Connector distilled` | bf16 | 2.86 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/text_encoders/ltx-2-19b-embeddings_connector_distill_bf16.safetensors)

---

## LoRA
*   [LTX-2-19b-LoRA-SPROUT](https://huggingface.co/oumoumad/LTX-2-19b-LoRA-SPROUT)

---

##  Workflow & Technical Notes
