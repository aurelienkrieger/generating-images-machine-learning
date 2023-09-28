# generating-images-machine-learning
Course about how to use generative models for AI art

# Overview

<img src="assets/generative models workflow.png" width="500" alt="generative model workflow">

## 1. Prompt engineering

**Key points**
- describe in a natural language and in the most detailed way the subject
- add keywords following the structure:
  - Medium
  - Style
  - Artist / Inspiration
  - Website	Resolution
  - Details
  - Color
  - Lighting
- use negative prompts
- ponderate keywords
- know how to play with parameters
- remix faces

**Tutorials from Stable Diffusion Art**

_prompts_

- [How to come up with good-prompts](https://stable-diffusion-art.com/how-to-come-up-with-good-prompts-for-ai-image-generation/)
- [Fine tune your images with simple prompting techniques](https://stable-diffusion-art.com/fine-tune-your-ai-images-with-these-simple-prompting-techniques/)
- [Important parameters](https://stable-diffusion-art.com/know-these-important-parameters-for-stunning-ai-images/)

_negative prompts_

- [How negative prompts work](https://stable-diffusion-art.com/how-negative-prompt-work/)
- [How to use negative prompts](https://stable-diffusion-art.com/how-to-use-negative-prompts/)

**Prompt generators**

- [Promptomania](https://promptomania.com/stable-diffusion-prompt-builder/)
- [Custom keyword organiser](https://docs.google.com/spreadsheets/d/1w953xYyb_6HoUXF_SiLdPkpA_IljhAjN31z6pnjKh1s/edit?usp=sharing)

**Parameters**

- Classifier Free Guidance (CFG) scale
- Sampling steps
- Image size
- Sampling method
- Seed
- Batch size

## 2. Generative models

### 2.1 Models family

**Stable Diffusion checkpoint models**

[Tutorial from Stable Diffusion Art](https://stable-diffusion-art.com/models/)

- Stable Diffusion v1.5: The official base model. Versatile in all styles
- Realistic Vision v2.0: Excel in generating photo-style realistic images
- Anything v5.0: Anime style
- SDXL Base 1.0: Stable Diffusion’s latest model

**other models**

- DALL-E
- MidJourney

**Stable Diffusion - functionalities**

- text-to-image (txt2img)
- image-to-image (img2img)
- depth-to-image (Depth2img)
- inpaiting
- text-to-video
- video-to-video
- Face restoration
- Regional prompting

**Models for additional control**

- Deforum
- controlNet
- Instruct Pix2Pix
- CodeFormer
- Real-ESRGAN
- GFPGAN
- [Controlnet QR Pattern](https://civitai.com/models/90940/controlnet-qr-pattern-qr-codes)
- [Controlnet QR Monster](https://huggingface.co/monster-labs/control_v1p_sd15_qrcode_monster)
- [Controlnet Brightness / Illumination](https://huggingface.co/ioclab/ioc-controlnet/tree/main/models)

**Post processing models**

- Upscalers

  _tutorials from Stable Diffusion Art_
  - [AI upscaler](https://stable-diffusion-art.com/ai-upscaler/)
  - [ControlNet upscale](https://stable-diffusion-art.com/controlnet-upscale/)

### 2.2 text2video

[Tutorial from Stable Diffusion Art](https://stable-diffusion-art.com/text-to-video/)

- Deforum
- ModelScope
- AnimateDiff


## 3. GUI

### 3.1 Online (demos & colabs)

- [Hugging Face v1.5](https://huggingface.co/spaces/runwayml/stable-diffusion-v1-5)
- [Hugging Face v2.1](https://huggingface.co/spaces/stabilityai/stable-diffusion)
- [Easy Diffusion](https://stablediffusion.gigantic.work/)
- [Disco Diffusion - Google Colab](https://colab.research.google.com/github/alembics/disco-diffusion/blob/main/Disco_Diffusion.ipynb)
- [Graviti](https://library.graviti.com/)
- [Illusion Diffusion (Monster QR)](https://huggingface.co/spaces/AP123/IllusionDiffusion)


### 3.1 Online (commercial platforms)

- [Runway](https://runwayml.com/)
- [Replicate](https://replicate.com/)
- [KREA](https://www.krea.ai/)
- [Playground AI](https://playgroundai.com/)
- [Dream Studio](https://beta.dreamstudio.ai/generate)
- [Mage space](https://www.mage.space/)

### 3.2 Local

_harder to install_
- [AUTOMATIC1111 – best features but a bit harder to install](https://github.com/AUTOMATIC1111/stable-diffusion-webui)
- [Diffusers](https://huggingface.co/docs/diffusers/index)
- [Sygil - Windows and Linus only](https://github.com/Sygil-Dev/sygil-webui)
- [ComfyGUI - nodal interface](https://github.com/comfyanonymous/ComfyUI)

_easier to install_
- [Easy Diffusion](https://easydiffusion.github.io/)
- [DiffusionBee - Mac only](https://diffusionbee.com/)
- [Draw things - Mac only](https://drawthings.ai/)
- [NMKD - Windows only](https://nmkd.itch.io/t2i-gui)

## 4. Model training

**Models & methods**
- Dreambooth
- LoRA
- LyCORIS
- Embedding

**Tutorials from Stable Diffusion Art**
- [Dreambooth](https://stable-diffusion-art.com/dreambooth/)
- [Embedding](https://stable-diffusion-art.com/embedding/)
- [LoRA](https://stable-diffusion-art.com/lora/)
- [Train LoRA](https://stable-diffusion-art.com/train-lora/)
