# Awesome LTX-2

A curated list of models, text encoders, and tools for the LTX-2 video generation suite.

## Models

LTX-2 models are available in various formats including full weights, transformers-only, and GGUF quantizations for efficient inference.

### Checkpoints
* **[Lightricks/LTX-2](https://huggingface.co/Lightricks/LTX-2)** - Official repository.

| Name | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `ltx-2-19b dev` | bf16 | 43.3 GB | [Link](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-dev.safetensors)
| `ltx-2-19b dev` | fp8 | 27.1 GB | [Link](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-dev-fp8.safetensors)
| `ltx-2-19b dev` | fp4 | 20 GB | [Link](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-dev-fp4.safetensors)
| `ltx-2-19b distilled` | bf16 | 43.3 GB | [Link](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-distilled.safetensors)
| `ltx-2-19b distilled` | fp8 | 27.1 GB | [Link](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-distilled-fp8.safetensors)

#### **Distilled LoRA**

| Rank | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `384` | bf16 | 7.67 GB | [Link](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-19b-distilled-lora-384.safetensors)
| `242` | bf16 | 4.88 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/loras/ltx-2-19b-distilled-lora-resized_dynamic_fro095_avg_rank_242_bf16.safetensors) |
| `175` | bf16 | 3.58 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/loras/ltx-2-19b-distilled-lora_resized_dynamic_fro09_avg_rank_175_bf16.safetensors) |
| `175` | fp8 | 1.79 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/loras/ltx-2-19b-distilled-lora_resized_dynamic_fro09_avg_rank_175_fp8.safetensors) |

#### **Spatial Upscaler** 
Required for current two-stage pipeline implementations in this repository. Download to `COMFYUI_ROOT_FOLDER/models/latent_upscale_models` folder.
  * [`ltx-2-spatial-upscaler-x2-1.0.safetensors`](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-spatial-upscaler-x2-1.0.safetensors)

#### **Temporal Upscaler** 
Required for current two-stage pipeline implementations in this repository. Download to `COMFYUI_ROOT_FOLDER/models/latent_upscale_models` folder.
  * [`ltx-2-temporal-upscaler-x2-1.0.safetensors`](https://huggingface.co/Lightricks/LTX-2/resolve/main/ltx-2-temporal-upscaler-x2-1.0.safetensors)


---

### GGUF Quantized Models
These models are optimized for lower memory usage. Note that in ComfyUI, these are typically loaded as transformer-only models.

<details>
  <summary>QuantStack</summary>
  
#### [QuantStack](https://huggingface.co/QuantStack/LTX-2-GGUF)

| Model | Quant | Size | Download |
| :--- | :---: | :---: | :---: |
| LTX-2-dev | Q2_K | 8.03 GB | [Download](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q2_K.gguf) |
| LTX-2-dev | Q3_K_M | 10.3 GB | [Download](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q3_K_M.gguf) |
| LTX-2-dev | Q3_K_S | 9.57 GB | [Download](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q3_K_S.gguf) |
| LTX-2-dev | Q4_K_M | 13.4 GB | [Download](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q4_K_M.gguf) |
| LTX-2-dev | Q4_K_S | 12.3 GB | [Download](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q4_K_S.gguf) |
| LTX-2-dev | Q5_K_M | 15 GB | [Download](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q5_K_M.gguf) |
| LTX-2-dev | Q5_K_S | 14.2 GB | [Download](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q5_K_S.gguf) |
| LTX-2-dev | Q6_K | 16.6 GB | [Download](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q6_K.gguf) |
| LTX-2-dev | Q8_0 | 21.1 GB | [Download](https://huggingface.co/QuantStack/LTX-2-GGUF/resolve/main/LTX-2-dev/LTX-2-dev-Q8_0.gguf) |

</details>

<details>
  <summary>Unsloth </summary>
  
#### [Unsloth GGUFs](https://huggingface.co/unsloth/LTX-2-GGUF)

| Model | Quant | Size | Download |
| :--- | :--- | :--- | :--- |
| ltx-2-19b-dev | BF16 | 37.8 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-BF16.gguf) |
| ltx-2-19b-dev | F16 | 37.8 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-F16.gguf) |
| ltx-2-19b-dev | Q2_K | 8.1 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q2_K.gguf) |
| ltx-2-19b-dev | Q3_K_L | 10.7 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q3_K_L.gguf) |
| ltx-2-19b-dev | Q3_K_M | 10.1 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q3_K_M.gguf) |
| ltx-2-19b-dev | Q3_K_S | 9.47 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q3_K_S.gguf) |
| ltx-2-19b-dev | Q4_0 | 11.3 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q4_0.gguf) |
| ltx-2-19b-dev | Q4_1 | 12.3 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q4_1.gguf) |
| ltx-2-19b-dev | Q4_K_M | 12.8 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q4_K_M.gguf) |
| ltx-2-19b-dev | Q4_K_S | 11.9 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q4_K_S.gguf) |
| ltx-2-19b-dev | Q5_0 | 13.7 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q5_0.gguf) |
| ltx-2-19b-dev | Q5_1 | 14.6 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q5_1.gguf) |
| ltx-2-19b-dev | Q5_K_M | 14.3 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q5_K_M.gguf) |
| ltx-2-19b-dev | Q5_K_S | 13.6 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q5_K_S.gguf) |
| ltx-2-19b-dev | Q6_K | 16 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q6_K.gguf) |
| ltx-2-19b-dev | Q8_0 | 20.4 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q8_0.gguf) |

</details>

<details>
  <summary>Vantage</summary>
  
#### [Vantage AI GGUFs](https://huggingface.co/vantagewithai/)

| Model | Quant | Size | Download |
| :--- | :--- | :--- | :--- |
| ltx-2-19b-dev | Q3_K_M | 9.96 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q3_K_M.gguf) |
| ltx-2-19b-dev | Q3_K_S | 9.28 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q3_K_S.gguf) |
| ltx-2-19b-dev | Q4_0 | 11.6 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q4_0.gguf) |
| ltx-2-19b-dev | Q4_1 | 12.4 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q4_1.gguf) |
| ltx-2-19b-dev | Q4_K_M | 12.8 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q4_K_M.gguf) |
| ltx-2-19b-dev | Q4_K_S | 11.8 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q4_K_S.gguf) |
| ltx-2-19b-dev | Q5_0 | 13.6 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q5_0.gguf) |
| ltx-2-19b-dev | Q5_1 | 14.5 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q5_1.gguf) |
| ltx-2-19b-dev | Q5_K_M | 14.4 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q5_K_M.gguf) |
| ltx-2-19b-dev | Q5_K_S | 13.5 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q5_K_S.gguf) |
| ltx-2-19b-dev | Q6_K | 15.9 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q6_K.gguf) |
| ltx-2-19b-dev | Q8_0 | 20.4 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q8_0.gguf) |
| ltx-2-19b-distilled | Q3_K_M | 9.96 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q3_K_M.gguf) |
| ltx-2-19b-distilled | Q3_K_S | 9.28 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q3_K_S.gguf) |
| ltx-2-19b-distilled | Q4_0 | 11.6 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q4_0.gguf) |
| ltx-2-19b-distilled | Q4_1 | 12.4 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q4_1.gguf) |
| ltx-2-19b-distilled | Q4_K_M | 12.8 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q4_K_M.gguf) |
| ltx-2-19b-distilled | Q4_K_S | 11.8 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q4_K_S.gguf) |
| ltx-2-19b-distilled | Q5_0 | 13.6 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q5_0.gguf) |
| ltx-2-19b-distilled | Q5_1 | 14.5 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q5_1.gguf) |
| ltx-2-19b-distilled | Q5_K_M | 14.4 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q5_K_M.gguf) |
| ltx-2-19b-distilled | Q5_K_S | 13.5 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q5_K_S.gguf) |
| ltx-2-19b-distilled | Q6_K | 15.9 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q6_K.gguf) |
| ltx-2-19b-distilled | Q8_0 | 20.4 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/distilled/ltx-2-19b-distilled-Q8_0.gguf) |

</details>
  
---

## Text Encoders

LTX-2 requires Gemma-3-12b variants.

### **Comfy-Org Optimized Encoders**
Official and optimized versions for ComfyUI.

| Model Name | Size | Download |
| :--- | :--- | :---: |
| `gemma_3_12B_it.safetensors` | 24.4 GB | [Link](https://huggingface.co/Comfy-Org/ltx-2/resolve/main/split_files/text_encoders/gemma_3_12B_it.safetensors?download=true) |
| `gemma_3_12B_it_fpmixed.safetensors` | 13.7 GB | [Link](https://huggingface.co/Comfy-Org/ltx-2/resolve/main/split_files/text_encoders/gemma_3_12B_it_fpmixed.safetensors?download=true) |
| `gemma_3_12B_it_fp8_scaled.safetensors` | 13.2 GB | [Link](https://huggingface.co/Comfy-Org/ltx-2/resolve/main/split_files/text_encoders/gemma_3_12B_it_fp8_scaled.safetensors?download=true) |
| `gemma_3_12B_it_fp4_mixed.safetensors` |  9.5 GB | [Link](https://huggingface.co/Comfy-Org/ltx-2/resolve/main/split_files/text_encoders/gemma_3_12B_it_fp4_mixed.safetensors?download=true) |

* `gemma_3_12B_it_fpmixed`: Experimental quant. Should be better than the fp8 scaled
* `gemma_3_12B_it_fp4_mixed`: 90% fp4 layers

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
| `ltx-2-19b dev` | bf16 | 37.8 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/diffusion_models/ltx-2-19b-dev_transformer_only_bf16.safetensors)
| `ltx-2-19b dev` | fp8 | 21.6 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/diffusion_models/ltx-2-19b-dev-fp8_transformer_only.safetensors)
| `ltx-2-19b distilled` | fp8 | 21.6 GB | [Link](https://huggingface.co/Kijai/LTXV2_comfy/resolve/main/diffusion_models/ltx-2-19b-distilled-fp8_transformer_only.safetensors)



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
  * [`ltx-2-19b-ic-lora-canny-control.safetensors`](https://huggingface.co/Lightricks/LTX-2-19b-IC-LoRA-Canny-Control/blob/main/ltx-2-19b-ic-lora-canny-control.safetensors)
  * [`ltx-2-19b-ic-lora-depth-control.safetensors`](https://huggingface.co/Lightricks/LTX-2-19b-IC-LoRA-Depth-Control/blob/main/ltx-2-19b-ic-lora-depth-control.safetensors)
  * [`ltx-2-19b-ic-lora-detailer.safetensors`](https://huggingface.co/Lightricks/LTX-2-19b-IC-LoRA-Detailer/blob/main/ltx-2-19b-ic-lora-detailer.safetensors)
  * [`ltx-2-19b-ic-lora-pose-control.safetensors`](https://huggingface.co/Lightricks/LTX-2-19b-IC-LoRA-Pose-Control/blob/main/ltx-2-19b-ic-lora-pose-control.safetensors)
  * [`ltx-2-19b-lora-camera-control-dolly-in.safetensors`](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Dolly-In/blob/main/ltx-2-19b-lora-camera-control-dolly-in.safetensors)
  * [`ltx-2-19b-lora-camera-control-dolly-left.safetensors`](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Dolly-Left/blob/main/ltx-2-19b-lora-camera-control-dolly-left.safetensors)
  * [`ltx-2-19b-lora-camera-control-dolly-out.safetensors`](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Dolly-Out/blob/main/ltx-2-19b-lora-camera-control-dolly-out.safetensors)
  * [`ltx-2-19b-lora-camera-control-dolly-right.safetensors`](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Dolly-Right/blob/main/ltx-2-19b-lora-camera-control-dolly-right.safetensors)
  * [`ltx-2-19b-lora-camera-control-jib-down.safetensors`](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Jib-Down/blob/main/ltx-2-19b-lora-camera-control-jib-down.safetensors)
  * [`ltx-2-19b-lora-camera-control-jib-up.safetensors`](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Jib-Up/blob/main/ltx-2-19b-lora-camera-control-jib-up.safetensors)
  * [`ltx-2-19b-lora-camera-control-static.safetensors`](https://huggingface.co/Lightricks/LTX-2-19b-LoRA-Camera-Control-Static/blob/main/ltx-2-19b-lora-camera-control-static.safetensors)


---

##  Workflow & Technical Notes

**Lightricks** official WF:
* [`Text to video full model`](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/LTX-2_T2V_Full_wLora.json)
* [`Text to video distilled model (Fast)`](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/LTX-2_T2V_Distilled_wLora.json)
* [`Image to video full model`](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/LTX-2_I2V_Full_wLora.json)
* [`Image to video distilled model (Fast)`](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/LTX-2_I2V_Distilled_wLora.json)
* [`Video to video detailer`](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/LTX-2_V2V_Detailer.json)
* [`IC-LoRA distilled model (depth + human pose + edges)`](https://raw.githubusercontent.com/Lightricks/ComfyUI-LTXVideo/refs/heads/master/example_workflows/LTX-2_ICLoRA_All_Distilled.json)



