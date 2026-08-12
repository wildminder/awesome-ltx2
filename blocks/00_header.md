# Awesome LTX-2

A curated list of models, text encoders, and tools for the LTX-2 video generation suite.

![ltx-logo](https://github.com/user-attachments/assets/3e5471d1-8f0c-4cce-96a5-f487919878ed)


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

