# Workflow for image generation

This page provides with an overview of the topics discussed during the course.

<img src="assets/generative models workflow.png" width="500" alt="generative model workflow">

[Stable Diffusion Art - how Stable Diffusion works](https://stable-diffusion-art.com/how-stable-diffusion-work/)

## 1. Prompt engineering

- prompt & parameters
- negative prompt
- prompt generators & boilerplates
- reverse prompting
- regional prompting

## 2. Models

- Checkpoint models
  - Text to Image (txt2img)
  - Image to Image (img2img)
  - Text to Video
  - Video to Video

- Post-processing models
  - Inpaiting
  - Outpainting
  - Face restoration
    - CodeFormer
    - GFPGAN
    - VAE
  - Upscaling
    - Real-ESRGAN
    - Latent upscalers
    - Lanczos (traditional upscaler)
  - Tiling

- Image to Image models
  - ControlNet
    - OpenPose
    - Depth
    - Canny
    - LineArt
    - QR pattern
  - Instruct Pix2Pix

- Animation
  - Deforum
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

[AUTOMATIC1111 complete guide from Stable Diffusion Art](https://stable-diffusion-art.com/automatic1111/)

## 4. Model training

- Dreambooth
- LoRA
- LyCORIS
- Embedding
- Hypernetworks
