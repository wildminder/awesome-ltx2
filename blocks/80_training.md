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


