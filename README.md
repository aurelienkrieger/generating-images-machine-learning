# generating-images-machine-learning
Course about how to use generative models for AI art

# Overview

<img src="assets/generative models workflow.png" width="500" alt="generative model workflow">

[Stable Diffusion Art - how Stable Diffusion works](https://stable-diffusion-art.com/how-stable-diffusion-work/)

## 1. Prompt engineering

- prompt & parameters
- negative prompt
- prompt generators & boilerplates
- reverse prompting

## 2. Models

**Popular functionalities**

- text-to-image (txt2img)
- image-to-image (img2img)
- depth-to-image (depth2img)
- inpaiting
- outpainting
- text-to-video
- video-to-video
- face restoration
- tiling
- upscaling
- regional prompting


### 2.1 Checkpoint models

**Stable Diffusion checkpoint models**

[Stable Diffusion Art - models](https://stable-diffusion-art.com/models/)

- Stable Diffusion v1.5: The official base model. Versatile in all styles
- Realistic Vision v2.0: Excel in generating photo-style realistic images
- Anything v5.0: Anime style
- SDXL Base 1.0: Stable Diffusion’s latest model

**other models**

- DALL-E
- MidJourney

### 2.2 Models for advanced control

**img2img**
- ControlNet
- Instruct Pix2Pix
- [Controlnet QR Pattern](https://civitai.com/models/90940/controlnet-qr-pattern-qr-codes)
- [Controlnet QR Monster](https://huggingface.co/monster-labs/control_v1p_sd15_qrcode_monster)
- [Controlnet Brightness / Illumination](https://huggingface.co/ioclab/ioc-controlnet/tree/main/models)

**Inpainting & outpainting**

_tutorials_
- [Stable Diffusion Art - inpainting](https://stable-diffusion-art.com/inpainting_basics/)
- [Stable Diffusion Art - outpainting](https://stable-diffusion-art.com/outpainting/)

**Face restoration**

- CodeFormer (faces restoration) 
- GFPGAN (faces restoration)
- VAE (faces restoration)

**Upscaling**

- Real-ESRGAN
- Latent upscalers
- Lanczos (traditional upscaler)

_tutorials_
- [Stable Diffusion Art - AI upscaler](https://stable-diffusion-art.com/ai-upscaler/)
- [Stable Diffusion Art - ControlNet upscale](https://stable-diffusion-art.com/controlnet-upscale/)

**Animation**

- Deforum
- AnimateDiff

_tutorials_
[Stable Diffusion Art - text2video](https://stable-diffusion-art.com/text-to-video/)


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

[AUTOMATIC1111 complete guide from Stable Diffusion Art](https://stable-diffusion-art.com/automatic1111/)

## 4. Model training

**Models & methods**
- Dreambooth
- LoRA
- LyCORIS
- Embedding
- Hypernetworks

**Tutorials from Stable Diffusion Art**
- [Dreambooth](https://stable-diffusion-art.com/dreambooth/)
- [Embedding](https://stable-diffusion-art.com/embedding/)
- [LoRA](https://stable-diffusion-art.com/lora/)
- [Train LoRA](https://stable-diffusion-art.com/train-lora/)
- [Hypernetworks](https://stable-diffusion-art.com/hypernetwork/)

**Resources**
- [Civitai, resource to download models](https://civitai.com/)