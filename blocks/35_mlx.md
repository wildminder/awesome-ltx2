<p id="mlx" align="center">◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇◆◇</p>

## ▓ MLX (Apple Silicon)

MLX conversions are **safetensors for Apple Silicon (Metal)** - a different runtime family from the CUDA builds above, not a GGUF variant. They load natively through `mlx-lm`, the `ltx-2-mlx` Python runtime, `ltx-2-mlx-swift` and **[mlx-serve](https://mlxserve.com)**. Every pack is **split per component** (`transformer-*`, `connector`, `vae_*`, `vocoder`, `audio_vae`, `spatial_upscaler_*`, `temporal_upscaler_*`, `gemma4-12b-ltx-v1/`), so you only download what your pipeline actually needs.

Quantized packs keep the **non-quantized layers in BF16**: the 4-bit / 8-bit payload is stored as packed `U32` tensors next to BF16 tensors and F32 scales, so the on-disk size stays well above a pure 4-bit / 8-bit model. The bit width and group size are recorded in each repo's `quantize_config.json` (`bits`, `group_size`, `only_transformer_blocks`).

<details>
  <summary><b>mlx-community</b> - LTX-2.5 (bf16)</summary>

**[`mlx-community/ltx-2.5-mlx`](https://huggingface.co/mlx-community/ltx-2.5-mlx)** - The reference MLX conversion of `Lightricks/LTX-2.5` - full bf16, no quantization. Ships **both** the `dev` and the `distilled` transformer plus the Gemma-4-12b text encoder, the connector, the whole VAE family and both upscalers.

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `transformer-dev.safetensors` | ![bf16][badge-bf16] | 37.99 GB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx/resolve/main/transformer-dev.safetensors) |
| `transformer-distilled.safetensors` | ![bf16][badge-bf16] | 37.99 GB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx/resolve/main/transformer-distilled.safetensors) |
| `connector.safetensors` | ![bf16][badge-bf16] | 6.34 GB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx/resolve/main/connector.safetensors) |
| `gemma4-12b-ltx-v1/model.safetensors` | ![bf16][badge-bf16] | 23.81 GB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx/resolve/main/gemma4-12b-ltx-v1/model.safetensors) |
| `vae_decoder.safetensors` | ![bf16][badge-bf16] | 814.35 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx/resolve/main/vae_decoder.safetensors) |
| `vae_decoder_pruna.safetensors` | ![bf16][badge-bf16] | 690.03 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx/resolve/main/vae_decoder_pruna.safetensors) |
| `vae_diffusion_decoder.safetensors` | ![bf16][badge-bf16] | 834.32 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx/resolve/main/vae_diffusion_decoder.safetensors) |
| `vae_encoder.safetensors` | ![bf16][badge-bf16] | 637.89 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx/resolve/main/vae_encoder.safetensors) |
| `vocoder.safetensors` | ![bf16][badge-bf16] | 258.31 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx/resolve/main/vocoder.safetensors) |
| `audio_vae.safetensors` | ![bf16][badge-bf16] | 106.51 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx/resolve/main/audio_vae.safetensors) |
| `duration_head.safetensors` | ![bf16][badge-bf16] | 3.81 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx/resolve/main/duration_head.safetensors) |
| `spatial_upscaler_x2_v1_1.safetensors` | ![bf16][badge-bf16] | 995.75 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx/resolve/main/spatial_upscaler_x2_v1_1.safetensors) |
| `temporal_upscaler_x2_v1_0.safetensors` | ![bf16][badge-bf16] | 261.95 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx/resolve/main/temporal_upscaler_x2_v1_0.safetensors) |

</details>

<details>
  <summary><b>mlx-community</b> - LTX-2.5 (q8)</summary>

**[`mlx-community/ltx-2.5-mlx-q8`](https://huggingface.co/mlx-community/ltx-2.5-mlx-q8)** - The **q8 text-encoder half** of the pack above - it deliberately ships **no transformer**: pair it with the bf16 `transformer-dev` / `transformer-distilled` from `mlx-community/ltx-2.5-mlx`. The Gemma-4-12b encoder is stored as packed `U32` at 8-bit.

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `connector.safetensors` | ![bf16][badge-bf16] | 6.34 GB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx-q8/resolve/main/connector.safetensors) |
| `gemma4-12b-ltx-v1/model-00001-of-00003.safetensors` | ![q8][badge-mlxq8] | 5.32 GB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx-q8/resolve/main/gemma4-12b-ltx-v1/model-00001-of-00003.safetensors) |
| `gemma4-12b-ltx-v1/model-00002-of-00003.safetensors` | ![q8][badge-mlxq8] | 5.32 GB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx-q8/resolve/main/gemma4-12b-ltx-v1/model-00002-of-00003.safetensors) |
| `gemma4-12b-ltx-v1/model-00003-of-00003.safetensors` | ![q8][badge-mlxq8] | 2.96 GB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx-q8/resolve/main/gemma4-12b-ltx-v1/model-00003-of-00003.safetensors) |
| `vae_decoder.safetensors` | ![bf16][badge-bf16] | 814.35 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx-q8/resolve/main/vae_decoder.safetensors) |
| `vae_decoder_pruna.safetensors` | ![bf16][badge-bf16] | 690.03 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx-q8/resolve/main/vae_decoder_pruna.safetensors) |
| `vae_diffusion_decoder.safetensors` | ![bf16][badge-bf16] | 834.32 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx-q8/resolve/main/vae_diffusion_decoder.safetensors) |
| `vae_encoder.safetensors` | ![bf16][badge-bf16] | 637.89 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx-q8/resolve/main/vae_encoder.safetensors) |
| `vocoder.safetensors` | ![bf16][badge-bf16] | 258.31 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx-q8/resolve/main/vocoder.safetensors) |
| `audio_vae.safetensors` | ![bf16][badge-bf16] | 106.51 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx-q8/resolve/main/audio_vae.safetensors) |
| `duration_head.safetensors` | ![bf16][badge-bf16] | 3.81 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx-q8/resolve/main/duration_head.safetensors) |
| `spatial_upscaler_x2_v1_1.safetensors` | ![bf16][badge-bf16] | 995.75 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx-q8/resolve/main/spatial_upscaler_x2_v1_1.safetensors) |
| `temporal_upscaler_x2_v1_0.safetensors` | ![bf16][badge-bf16] | 261.95 MB | [![][gh-mlx-community]](https://huggingface.co/mlx-community/ltx-2.5-mlx-q8/resolve/main/temporal_upscaler_x2_v1_0.safetensors) |

</details>

<details>
  <summary><b>dgrauet</b> - LTX-2.3 (bf16)</summary>

**[`dgrauet/ltx-2.3-mlx`](https://huggingface.co/dgrauet/ltx-2.3-mlx)** - Reference bf16 MLX conversion of LTX-2.3. Carries the `dev`, `distilled` and `distilled-1.1` transformers plus both rank-384 distilled LoRAs (`384` and `384-1.1`).

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `transformer-dev.safetensors` | ![bf16][badge-bf16] | 37.99 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx/resolve/main/transformer-dev.safetensors) |
| `transformer-distilled-1.1.safetensors` | ![bf16][badge-bf16] | 37.99 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx/resolve/main/transformer-distilled-1.1.safetensors) |
| `transformer-distilled.safetensors` | ![bf16][badge-bf16] | 37.99 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx/resolve/main/transformer-distilled.safetensors) |
| `connector.safetensors` | ![bf16][badge-bf16] | 6.34 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx/resolve/main/connector.safetensors) |
| `ltx-2.3-22b-distilled-lora-384-1.1.safetensors` | ![bf16][badge-bf16] | 7.61 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx/resolve/main/ltx-2.3-22b-distilled-lora-384-1.1.safetensors) |
| `ltx-2.3-22b-distilled-lora-384.safetensors` | ![bf16][badge-bf16] | 7.61 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx/resolve/main/ltx-2.3-22b-distilled-lora-384.safetensors) |
| `vae_decoder.safetensors` | ![bf16][badge-bf16] | 814.35 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx/resolve/main/vae_decoder.safetensors) |
| `vae_encoder.safetensors` | ![bf16][badge-bf16] | 637.89 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx/resolve/main/vae_encoder.safetensors) |
| `vocoder.safetensors` | ![bf16][badge-bf16] | 258.31 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx/resolve/main/vocoder.safetensors) |
| `audio_vae.safetensors` | ![bf16][badge-bf16] | 106.51 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx/resolve/main/audio_vae.safetensors) |
| `spatial_upscaler_x1_5_v1_0.safetensors` | ![bf16][badge-bf16] | 1.09 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx/resolve/main/spatial_upscaler_x1_5_v1_0.safetensors) |
| `spatial_upscaler_x2_v1_1.safetensors` | ![bf16][badge-bf16] | 995.75 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx/resolve/main/spatial_upscaler_x2_v1_1.safetensors) |
| `temporal_upscaler_x2_v1_0.safetensors` | ![bf16][badge-bf16] | 261.95 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx/resolve/main/temporal_upscaler_x2_v1_0.safetensors) |

</details>

<details>
  <summary><b>dgrauet</b> - LTX-2.3 (q4)</summary>

**[`dgrauet/ltx-2.3-mlx-q4`](https://huggingface.co/dgrauet/ltx-2.3-mlx-q4)** - 4-bit MLX pack (`bits: 4`, `group_size: 64`, transformer blocks only) - the most downloaded MLX conversion of LTX-2.3. Still carries the bf16 rank-384 distilled LoRAs.

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `transformer-dev.safetensors` | ![q4][badge-mlxq4] | 11.32 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q4/resolve/main/transformer-dev.safetensors) |
| `transformer-distilled-1.1.safetensors` | ![q4][badge-mlxq4] | 11.32 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q4/resolve/main/transformer-distilled-1.1.safetensors) |
| `transformer-distilled.safetensors` | ![q4][badge-mlxq4] | 11.32 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q4/resolve/main/transformer-distilled.safetensors) |
| `connector.safetensors` | ![bf16][badge-bf16] | 6.34 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q4/resolve/main/connector.safetensors) |
| `ltx-2.3-22b-distilled-lora-384-1.1.safetensors` | ![bf16][badge-bf16] | 7.61 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q4/resolve/main/ltx-2.3-22b-distilled-lora-384-1.1.safetensors) |
| `ltx-2.3-22b-distilled-lora-384.safetensors` | ![bf16][badge-bf16] | 7.61 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q4/resolve/main/ltx-2.3-22b-distilled-lora-384.safetensors) |
| `vae_decoder.safetensors` | ![bf16][badge-bf16] | 814.35 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q4/resolve/main/vae_decoder.safetensors) |
| `vae_encoder.safetensors` | ![bf16][badge-bf16] | 637.89 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q4/resolve/main/vae_encoder.safetensors) |
| `vocoder.safetensors` | ![bf16][badge-bf16] | 258.31 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q4/resolve/main/vocoder.safetensors) |
| `audio_vae.safetensors` | ![bf16][badge-bf16] | 106.51 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q4/resolve/main/audio_vae.safetensors) |
| `spatial_upscaler_x1_5_v1_0.safetensors` | ![bf16][badge-bf16] | 1.09 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q4/resolve/main/spatial_upscaler_x1_5_v1_0.safetensors) |
| `spatial_upscaler_x2_v1_1.safetensors` | ![bf16][badge-bf16] | 995.75 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q4/resolve/main/spatial_upscaler_x2_v1_1.safetensors) |
| `temporal_upscaler_x2_v1_0.safetensors` | ![bf16][badge-bf16] | 261.95 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q4/resolve/main/temporal_upscaler_x2_v1_0.safetensors) |

</details>

<details>
  <summary><b>dgrauet</b> - LTX-2.3 (q8)</summary>

**[`dgrauet/ltx-2.3-mlx-q8`](https://huggingface.co/dgrauet/ltx-2.3-mlx-q8)** - 8-bit MLX pack (`bits: 8`, `group_size: 64`, transformer blocks only) - the middle ground between the bf16 and 4-bit packs.

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `transformer-dev.safetensors` | ![q8][badge-mlxq8] | 20.60 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q8/resolve/main/transformer-dev.safetensors) |
| `transformer-distilled-1.1.safetensors` | ![q8][badge-mlxq8] | 20.60 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q8/resolve/main/transformer-distilled-1.1.safetensors) |
| `transformer-distilled.safetensors` | ![q8][badge-mlxq8] | 20.60 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q8/resolve/main/transformer-distilled.safetensors) |
| `connector.safetensors` | ![bf16][badge-bf16] | 6.34 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q8/resolve/main/connector.safetensors) |
| `ltx-2.3-22b-distilled-lora-384-1.1.safetensors` | ![bf16][badge-bf16] | 7.61 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q8/resolve/main/ltx-2.3-22b-distilled-lora-384-1.1.safetensors) |
| `ltx-2.3-22b-distilled-lora-384.safetensors` | ![bf16][badge-bf16] | 7.61 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q8/resolve/main/ltx-2.3-22b-distilled-lora-384.safetensors) |
| `vae_decoder.safetensors` | ![bf16][badge-bf16] | 814.35 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q8/resolve/main/vae_decoder.safetensors) |
| `vae_encoder.safetensors` | ![bf16][badge-bf16] | 637.89 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q8/resolve/main/vae_encoder.safetensors) |
| `vocoder.safetensors` | ![bf16][badge-bf16] | 258.31 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q8/resolve/main/vocoder.safetensors) |
| `audio_vae.safetensors` | ![bf16][badge-bf16] | 106.51 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q8/resolve/main/audio_vae.safetensors) |
| `spatial_upscaler_x1_5_v1_0.safetensors` | ![bf16][badge-bf16] | 1.09 GB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q8/resolve/main/spatial_upscaler_x1_5_v1_0.safetensors) |
| `spatial_upscaler_x2_v1_1.safetensors` | ![bf16][badge-bf16] | 995.75 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q8/resolve/main/spatial_upscaler_x2_v1_1.safetensors) |
| `temporal_upscaler_x2_v1_0.safetensors` | ![bf16][badge-bf16] | 261.95 MB | [![][gh-dgrauet]](https://huggingface.co/dgrauet/ltx-2.3-mlx-q8/resolve/main/temporal_upscaler_x2_v1_0.safetensors) |

</details>

<details>
  <summary><b>ddalcu</b> - LTX-2.5 (q4)</summary>

**[`ddalcu/LTX-2.5-MLX-Serve-4bit`](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-4bit)** - Self-contained 4-bit pack for **[mlx-serve](https://mlxserve.com)**, the native Zig MLX server for Apple Silicon. The text encoder is inside the pack, so nothing else downloads. Ships a `split_model.json` manifest.

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `transformer-dev.safetensors` | ![q4][badge-mlxq4] | 11.32 GB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-4bit/resolve/main/transformer-dev.safetensors) |
| `transformer-distilled.safetensors` | ![q4][badge-mlxq4] | 11.32 GB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-4bit/resolve/main/transformer-distilled.safetensors) |
| `connector.safetensors` | ![bf16][badge-bf16] | 6.34 GB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-4bit/resolve/main/connector.safetensors) |
| `gemma4-12b-ltx-v1/model.safetensors` | ![q4][badge-mlxq4] | 6.70 GB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-4bit/resolve/main/gemma4-12b-ltx-v1/model.safetensors) |
| `vae_decoder.safetensors` | ![bf16][badge-bf16] | 814.35 MB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-4bit/resolve/main/vae_decoder.safetensors) |
| `vae_encoder.safetensors` | ![bf16][badge-bf16] | 637.89 MB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-4bit/resolve/main/vae_encoder.safetensors) |
| `vocoder.safetensors` | ![bf16][badge-bf16] | 258.31 MB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-4bit/resolve/main/vocoder.safetensors) |
| `audio_vae.safetensors` | ![bf16][badge-bf16] | 106.51 MB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-4bit/resolve/main/audio_vae.safetensors) |
| `spatial_upscaler_x2_v1_1.safetensors` | ![bf16][badge-bf16] | 995.75 MB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-4bit/resolve/main/spatial_upscaler_x2_v1_1.safetensors) |
| `temporal_upscaler_x2_v1_0.safetensors` | ![bf16][badge-bf16] | 261.95 MB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-4bit/resolve/main/temporal_upscaler_x2_v1_0.safetensors) |

</details>

<details>
  <summary><b>ddalcu</b> - LTX-2.5 (q8)</summary>

**[`ddalcu/LTX-2.5-MLX-Serve-8bit`](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-8bit)** - The 8-bit sibling of the mlx-serve pack - same layout, wider payload, plus the `vae_diffusion_decoder`.

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `transformer-dev.safetensors` | ![q8][badge-mlxq8] | 20.60 GB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-8bit/resolve/main/transformer-dev.safetensors) |
| `transformer-distilled.safetensors` | ![q8][badge-mlxq8] | 20.60 GB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-8bit/resolve/main/transformer-distilled.safetensors) |
| `connector.safetensors` | ![bf16][badge-bf16] | 6.34 GB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-8bit/resolve/main/connector.safetensors) |
| `gemma4-12b-ltx-v1/model.safetensors` | ![q8][badge-mlxq8] | 12.65 GB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-8bit/resolve/main/gemma4-12b-ltx-v1/model.safetensors) |
| `vae_decoder.safetensors` | ![bf16][badge-bf16] | 814.35 MB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-8bit/resolve/main/vae_decoder.safetensors) |
| `vae_diffusion_decoder.safetensors` | ![bf16][badge-bf16] | 834.32 MB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-8bit/resolve/main/vae_diffusion_decoder.safetensors) |
| `vae_encoder.safetensors` | ![bf16][badge-bf16] | 637.89 MB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-8bit/resolve/main/vae_encoder.safetensors) |
| `vocoder.safetensors` | ![bf16][badge-bf16] | 258.31 MB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-8bit/resolve/main/vocoder.safetensors) |
| `audio_vae.safetensors` | ![bf16][badge-bf16] | 106.51 MB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-8bit/resolve/main/audio_vae.safetensors) |
| `spatial_upscaler_x2_v1_1.safetensors` | ![bf16][badge-bf16] | 995.75 MB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-8bit/resolve/main/spatial_upscaler_x2_v1_1.safetensors) |
| `temporal_upscaler_x2_v1_0.safetensors` | ![bf16][badge-bf16] | 261.95 MB | [![][gh-ddalcu]](https://huggingface.co/ddalcu/LTX-2.5-MLX-Serve-8bit/resolve/main/temporal_upscaler_x2_v1_0.safetensors) |

</details>

<details>
  <summary><b>MrMofer</b> - LTX-2.5 (q8)</summary>

**[`MrMofer/ltx-2.5-mlx-q8`](https://huggingface.co/MrMofer/ltx-2.5-mlx-q8)** - 8-bit MLX conversion of LTX-2.5 with the rank-450 distilled LoRA included. The text encoder lives in a `text_encoder/` folder rather than `gemma4-12b-ltx-v1/`.

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `transformer-dev.safetensors` | ![q8][badge-mlxq8] | 20.60 GB | [![][gh-MrMofer]](https://huggingface.co/MrMofer/ltx-2.5-mlx-q8/resolve/main/transformer-dev.safetensors) |
| `transformer-distilled.safetensors` | ![q8][badge-mlxq8] | 20.60 GB | [![][gh-MrMofer]](https://huggingface.co/MrMofer/ltx-2.5-mlx-q8/resolve/main/transformer-distilled.safetensors) |
| `connector.safetensors` | ![bf16][badge-bf16] | 6.34 GB | [![][gh-MrMofer]](https://huggingface.co/MrMofer/ltx-2.5-mlx-q8/resolve/main/connector.safetensors) |
| `text_encoder/model.safetensors` | ![q4][badge-mlxq4] | 8.15 GB | [![][gh-MrMofer]](https://huggingface.co/MrMofer/ltx-2.5-mlx-q8/resolve/main/text_encoder/model.safetensors) |
| `ltx-2.5-22b-distilled-lora-450.safetensors` | ![bf16][badge-bf16] | 8.90 GB | [![][gh-MrMofer]](https://huggingface.co/MrMofer/ltx-2.5-mlx-q8/resolve/main/ltx-2.5-22b-distilled-lora-450.safetensors) |
| `vae_decoder.safetensors` | ![bf16][badge-bf16] | 814.35 MB | [![][gh-MrMofer]](https://huggingface.co/MrMofer/ltx-2.5-mlx-q8/resolve/main/vae_decoder.safetensors) |
| `vae_encoder.safetensors` | ![bf16][badge-bf16] | 637.89 MB | [![][gh-MrMofer]](https://huggingface.co/MrMofer/ltx-2.5-mlx-q8/resolve/main/vae_encoder.safetensors) |
| `vocoder.safetensors` | ![bf16][badge-bf16] | 258.31 MB | [![][gh-MrMofer]](https://huggingface.co/MrMofer/ltx-2.5-mlx-q8/resolve/main/vocoder.safetensors) |
| `audio_vae.safetensors` | ![bf16][badge-bf16] | 106.51 MB | [![][gh-MrMofer]](https://huggingface.co/MrMofer/ltx-2.5-mlx-q8/resolve/main/audio_vae.safetensors) |
| `duration_head.safetensors` | ![bf16][badge-bf16] | 3.81 MB | [![][gh-MrMofer]](https://huggingface.co/MrMofer/ltx-2.5-mlx-q8/resolve/main/duration_head.safetensors) |
| `spatial_upscaler_x2.safetensors` | ![bf16][badge-bf16] | 995.74 MB | [![][gh-MrMofer]](https://huggingface.co/MrMofer/ltx-2.5-mlx-q8/resolve/main/spatial_upscaler_x2.safetensors) |
| `temporal_upscaler_x2.safetensors` | ![bf16][badge-bf16] | 261.94 MB | [![][gh-MrMofer]](https://huggingface.co/MrMofer/ltx-2.5-mlx-q8/resolve/main/temporal_upscaler_x2.safetensors) |

</details>

<details>
  <summary><b>notapalindrome</b> - LTX-2.3 (q4)</summary>

**[`notapalindrome/ltx23-mlx-av-q4`](https://huggingface.co/notapalindrome/ltx23-mlx-av-q4)** - 4-bit MLX conversion of LTX-2.3 with joint **audio + video** (`mlx-av`). Quantizes the whole model, not just the transformer blocks.

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `transformer.safetensors` | ![q4][badge-mlxq4] | 11.35 GB | [![][gh-notapalindrome]](https://huggingface.co/notapalindrome/ltx23-mlx-av-q4/resolve/main/transformer.safetensors) |
| `connector.safetensors` | ![bf16][badge-bf16] | 6.34 GB | [![][gh-notapalindrome]](https://huggingface.co/notapalindrome/ltx23-mlx-av-q4/resolve/main/connector.safetensors) |
| `vae_decoder.safetensors` | ![bf16][badge-bf16] | 814.35 MB | [![][gh-notapalindrome]](https://huggingface.co/notapalindrome/ltx23-mlx-av-q4/resolve/main/vae_decoder.safetensors) |
| `vae_encoder.safetensors` | ![bf16][badge-bf16] | 637.88 MB | [![][gh-notapalindrome]](https://huggingface.co/notapalindrome/ltx23-mlx-av-q4/resolve/main/vae_encoder.safetensors) |
| `vocoder.safetensors` | ![bf16][badge-bf16] | 258.30 MB | [![][gh-notapalindrome]](https://huggingface.co/notapalindrome/ltx23-mlx-av-q4/resolve/main/vocoder.safetensors) |
| `audio_vae.safetensors` | ![bf16][badge-bf16] | 63.84 MB | [![][gh-notapalindrome]](https://huggingface.co/notapalindrome/ltx23-mlx-av-q4/resolve/main/audio_vae.safetensors) |
| `spatial_upscaler_x1_5_v1_0.safetensors` | ![bf16][badge-bf16] | 1.09 GB | [![][gh-notapalindrome]](https://huggingface.co/notapalindrome/ltx23-mlx-av-q4/resolve/main/spatial_upscaler_x1_5_v1_0.safetensors) |
| `spatial_upscaler_x2_v1_1.safetensors` | ![bf16][badge-bf16] | 995.74 MB | [![][gh-notapalindrome]](https://huggingface.co/notapalindrome/ltx23-mlx-av-q4/resolve/main/spatial_upscaler_x2_v1_1.safetensors) |
| `upsampler.safetensors` | ![bf16][badge-bf16] | 995.74 MB | [![][gh-notapalindrome]](https://huggingface.co/notapalindrome/ltx23-mlx-av-q4/resolve/main/upsampler.safetensors) |
| `temporal_upscaler_x2_v1_0.safetensors` | ![bf16][badge-bf16] | 261.94 MB | [![][gh-notapalindrome]](https://huggingface.co/notapalindrome/ltx23-mlx-av-q4/resolve/main/temporal_upscaler_x2_v1_0.safetensors) |

</details>

<details>
  <summary><b>xocialize</b> - LTX-2.3 (bf16)</summary>

**[`xocialize/ltx-2.3-mlx`](https://huggingface.co/xocialize/ltx-2.3-mlx)** - bf16 MLX conversion of LTX-2.3 carrying the `distilled` transformer only - the compact option for the `ltx-2-mlx` Python runtime.

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `transformer-distilled.safetensors` | ![bf16][badge-bf16] | 37.99 GB | [![][gh-xocialize]](https://huggingface.co/xocialize/ltx-2.3-mlx/resolve/main/transformer-distilled.safetensors) |
| `connector.safetensors` | ![bf16][badge-bf16] | 6.34 GB | [![][gh-xocialize]](https://huggingface.co/xocialize/ltx-2.3-mlx/resolve/main/connector.safetensors) |
| `vae_decoder.safetensors` | ![bf16][badge-bf16] | 814.35 MB | [![][gh-xocialize]](https://huggingface.co/xocialize/ltx-2.3-mlx/resolve/main/vae_decoder.safetensors) |
| `vae_decoder_pruna.safetensors` | ![bf16][badge-bf16] | 690.03 MB | [![][gh-xocialize]](https://huggingface.co/xocialize/ltx-2.3-mlx/resolve/main/vae_decoder_pruna.safetensors) |
| `vae_encoder.safetensors` | ![bf16][badge-bf16] | 637.89 MB | [![][gh-xocialize]](https://huggingface.co/xocialize/ltx-2.3-mlx/resolve/main/vae_encoder.safetensors) |
| `vocoder.safetensors` | ![bf16][badge-bf16] | 258.31 MB | [![][gh-xocialize]](https://huggingface.co/xocialize/ltx-2.3-mlx/resolve/main/vocoder.safetensors) |
| `audio_vae.safetensors` | ![bf16][badge-bf16] | 106.51 MB | [![][gh-xocialize]](https://huggingface.co/xocialize/ltx-2.3-mlx/resolve/main/audio_vae.safetensors) |
| `spatial_upscaler_x1_5_v1_0.safetensors` | ![bf16][badge-bf16] | 1.09 GB | [![][gh-xocialize]](https://huggingface.co/xocialize/ltx-2.3-mlx/resolve/main/spatial_upscaler_x1_5_v1_0.safetensors) |
| `spatial_upscaler_x2_v1_1.safetensors` | ![bf16][badge-bf16] | 995.75 MB | [![][gh-xocialize]](https://huggingface.co/xocialize/ltx-2.3-mlx/resolve/main/spatial_upscaler_x2_v1_1.safetensors) |
| `temporal_upscaler_x2_v1_0.safetensors` | ![bf16][badge-bf16] | 261.95 MB | [![][gh-xocialize]](https://huggingface.co/xocialize/ltx-2.3-mlx/resolve/main/temporal_upscaler_x2_v1_0.safetensors) |

</details>

<details>
  <summary><b>MLXBits</b> - LTX-2.3 (q4)</summary>

**[`MLXBits/ltx-2.3-10eros-v1.3-dmd-mlx-q4`](https://huggingface.co/MLXBits/ltx-2.3-10eros-v1.3-dmd-mlx-q4)** - 4-bit MLX conversion of the **10Eros v1.3 DMD** distilled LTX-2.3 merge (`bits: 4`, `group_size: 32`).

| Component | Precision | Size | Download |
| :--- | :---: | :---: | :---: |
| `transformer-distilled.safetensors` | ![q4][badge-mlxq4] | 12.47 GB | [![][gh-MLXBits]](https://huggingface.co/MLXBits/ltx-2.3-10eros-v1.3-dmd-mlx-q4/resolve/main/transformer-distilled.safetensors) |
| `connector.safetensors` | ![bf16][badge-bf16] | 6.34 GB | [![][gh-MLXBits]](https://huggingface.co/MLXBits/ltx-2.3-10eros-v1.3-dmd-mlx-q4/resolve/main/connector.safetensors) |
| `vae_decoder.safetensors` | ![bf16][badge-bf16] | 814.35 MB | [![][gh-MLXBits]](https://huggingface.co/MLXBits/ltx-2.3-10eros-v1.3-dmd-mlx-q4/resolve/main/vae_decoder.safetensors) |
| `vae_encoder.safetensors` | ![bf16][badge-bf16] | 637.89 MB | [![][gh-MLXBits]](https://huggingface.co/MLXBits/ltx-2.3-10eros-v1.3-dmd-mlx-q4/resolve/main/vae_encoder.safetensors) |
| `vocoder.safetensors` | ![bf16][badge-bf16] | 258.31 MB | [![][gh-MLXBits]](https://huggingface.co/MLXBits/ltx-2.3-10eros-v1.3-dmd-mlx-q4/resolve/main/vocoder.safetensors) |
| `audio_vae.safetensors` | ![bf16][badge-bf16] | 106.51 MB | [![][gh-MLXBits]](https://huggingface.co/MLXBits/ltx-2.3-10eros-v1.3-dmd-mlx-q4/resolve/main/audio_vae.safetensors) |
| `spatial_upscaler_x1_5_v1_0.safetensors` | ![bf16][badge-bf16] | 1.09 GB | [![][gh-MLXBits]](https://huggingface.co/MLXBits/ltx-2.3-10eros-v1.3-dmd-mlx-q4/resolve/main/spatial_upscaler_x1_5_v1_0.safetensors) |
| `spatial_upscaler_x2_v1_1.safetensors` | ![bf16][badge-bf16] | 995.75 MB | [![][gh-MLXBits]](https://huggingface.co/MLXBits/ltx-2.3-10eros-v1.3-dmd-mlx-q4/resolve/main/spatial_upscaler_x2_v1_1.safetensors) |
| `temporal_upscaler_x2_v1_0.safetensors` | ![bf16][badge-bf16] | 261.95 MB | [![][gh-MLXBits]](https://huggingface.co/MLXBits/ltx-2.3-10eros-v1.3-dmd-mlx-q4/resolve/main/temporal_upscaler_x2_v1_0.safetensors) |

</details>
