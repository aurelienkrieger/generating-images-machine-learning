# Models

## Overview

_types of models_
- checkpoint models
- embeddings (textural inversion)
- LoRA models
- hypernetworks

_file extensions_
- .ckpt
- .pt
- .safetensors
- diffusers models (folders)

_file variants_
- pruned
- full
- EMA-only
- fp16
- fp32

### Checkpoint models

- Text to Image
- Image to Image
- Text to Video
- Image to Video
- Video to Video

### Models for advanced control

- Refiners
- Inpaiting
- Outpainting
- Face restoration
  - CodeFormer
  - GFPGAN
- Upscaling
  - Real-ESRGAN
  - Latent upscalers
  - Lanczos (traditional upscaler)
- Image to Image
  - ControlNet
    - OpenPose
    - Depth
    - Canny
    - LineArt
    - IP-Adapter
    - QR Pattern
  - Instruct Pix2Pix
- Tiling

### Customize models

- VAE
- Embedding
- Dreambooth
- LoRA
- LyCORIS
- Hypernetworks

## Tutorials & resources

### Checkpoint models

**Stable Diffusion checkpoint models**

[Invoke AI models](https://models.invoke.ai/)

- Stable Diffusion v1.5 (Stable Diffusion base model)
  - [model page](https://huggingface.co/runwayml/stable-diffusion-v1-5)
  - [download link](https://huggingface.co/runwayml/stable-diffusion-v1-5/resolve/main/v1-5-pruned.safetensors)
  - [download link - inpainting](https://huggingface.co/runwayml/stable-diffusion-inpainting/resolve/main/sd-v1-5-inpainting.ckpt)
- SDXL v1.0 (Stable Diffusion’s latest model)
  - [model page](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0)
  - [download link](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0/resolve/main/sd_xl_base_1.0_0.9vae.safetensors)
  - [download link - refiner](https://huggingface.co/stabilityai/stable-diffusion-xl-refiner-1.0/resolve/main/sd_xl_refiner_1.0_0.9vae.safetensors)
- OpenJourney (include 'mdjrny-v4 style' in prompt)
  - [model page](https://huggingface.co/prompthero/openjourney)
  - [download link](https://huggingface.co/prompthero/openjourney/resolve/main/mdjrny-v4.safetensors)
- Juggernaut
  - [model page](https://civitai.com/models/46422)
  - [download link](https://civitai.com/api/download/models/127207?type=Model&format=SafeTensor&size=pruned&fp=fp16)
  - [download link - inpainting](https://civitai.com/api/download/models/129549?type=Model&format=SafeTensor&size=full&fp=fp32)
- Realistic Vision v5.1 (photo-style realistic images)
  - [model page](https://civitai.com/models/4201/realistic-vision-v20)
  - [download link](https://civitai.com/api/download/models/130072?type=Model&format=SafeTensor&size=pruned&fp=fp16)
  - [download link - inpainting](https://civitai.com/api/download/models/130090)
- Fantasy and Art by Zovya for InvokeAI
  - [model page](https://huggingface.co/Hipsterusername/InvokeAI_Fantasy_and_Art_by_Zovya)


**other models**

- DALL-E
- MidJourney

### Models for advanced control

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
- CodeFormer
- GFPGAN
- VAE
- Roop (Face swap)
  - [original project page](https://github.com/s0md3v/roop)
  - [AUTOMATIC1111 extension](https://github.com/s0md3v/sd-webui-roop)

**Upscaling**

- Real-ESRGAN
- Latent upscalers
- Lanczos (traditional upscaler)

_tutorials_
- [Stable Diffusion Art - AI upscaler](https://stable-diffusion-art.com/ai-upscaler/)
- [Stable Diffusion Art - ControlNet upscale](https://stable-diffusion-art.com/controlnet-upscale/)

**Embedding**

- [EasyNegative](https://civitai.com/models/7808/easynegative)

**Animation**

- Deforum
- AnimateDiff

_tutorials_
- [Stable Diffusion Art - text2video](https://stable-diffusion-art.com/text-to-video/)


## Resources
- [Civitai, resource to download models](https://civitai.com/models)
