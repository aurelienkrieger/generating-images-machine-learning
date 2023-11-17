# Resources for Models

## Useful links

### Stable Diffusion checkpoint models

- [Invoke AI models](https://models.invoke.ai/)
- [Civitai, resource to download models](https://civitai.com/models)
- [Hugging Face, a community-driven database of models, datasets, applications](https://huggingface.co/)

- Stable Diffusion v1.5
  - [model page](https://huggingface.co/runwayml/stable-diffusion-v1-5)
  - [download link](https://huggingface.co/runwayml/stable-diffusion-v1-5/resolve/main/v1-5-pruned.safetensors)
  - [download link - inpainting](https://huggingface.co/runwayml/stable-diffusion-inpainting/resolve/main/sd-v1-5-inpainting.ckpt)
- SDXL v1.0
  - [model page](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0)
  - [download link](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0/resolve/main/sd_xl_base_1.0_0.9vae.safetensors)
  - [download link - refiner](https://huggingface.co/stabilityai/stable-diffusion-xl-refiner-1.0/resolve/main/sd_xl_refiner_1.0_0.9vae.safetensors)

### Selection of Fine-tuned models

#### Trained & Merged models

- Juggernaut (use with separate VAE)
  - [model page](https://civitai.com/models/46422)
  - [download link](https://civitai.com/api/download/models/127207?type=Model&format=SafeTensor&size=pruned&fp=fp16)
  - [download link - inpainting](https://civitai.com/api/download/models/129549?type=Model&format=SafeTensor&size=full&fp=fp32)
- Realistic Vision v5.1 (photo-style realistic images)
  - [model page](https://civitai.com/models/4201/realistic-vision-v20)
  - [download link](https://civitai.com/api/download/models/130072?type=Model&format=SafeTensor&size=pruned&fp=fp16)
  - [download link - inpainting](https://civitai.com/api/download/models/130090)
- Fantasy and Art by Zovya for InvokeAI
  - [model page](https://huggingface.co/Hipsterusername/InvokeAI_Fantasy_and_Art_by_Zovya)
- DreamShaper
  - [model page](https://civitai.com/models/4384/dreamshaper)
  - [download link](https://civitai.com/api/download/models/128713?type=Model&format=SafeTensor&size=pruned&fp=fp16)
  - [download link - inpainting](https://civitai.com/api/download/models/131004)
- OpenJourney (include 'mdjrny-v4 style' in prompt)
  - [model page](https://huggingface.co/prompthero/openjourney)
  - [download link](https://huggingface.co/prompthero/openjourney/resolve/main/mdjrny-v4.safetensors)

#### LoRA models

- [epi_noiseoffset - LoRA model for better contrast and darker images](https://civitai.com/models/13941/epinoiseoffset)
- [LoRA Age Slider](https://civitai.com/models/128417/age-slider)
- [LoRA Skin Tone Slider](https://civitai.com/models/112594/skin-tone-slider-lora)
- [LoRA Gender Slider](https://civitai.com/models/112988/gender-slider-lora)
- [LoRA Muscle Slider](https://civitai.com/models/112658/muscle-slider-lora)

#### Embedding

- [EasyNegative](https://civitai.com/models/7808/easynegative)

### Other models

- [DALL-E](https://openai.com/dall-e-3)
- [MidJourney](https://www.midjourney.com/)
- [Google's Imagen](https://imagen.research.google/)

### Models for advanced control

#### img2img

- ControlNet
  - [ControlNet tutorial from Stable Diffusion art](https://stable-diffusion-art.com/controlnet/)
  - [ControlNet with SDXL tutorial from Stable Diffusion art](https://stable-diffusion-art.com/controlnet-sdxl/)
- [Instruct Pix2Pix](https://www.timothybrooks.com/instruct-pix2pix)
- [T2I Adapter](https://github.com/TencentARC/T2I-Adapter)
- [Controlnet QR Pattern](https://civitai.com/models/90940/controlnet-qr-pattern-qr-codes)
- [Controlnet QR Monster](https://huggingface.co/monster-labs/control_v1p_sd15_qrcode_monster)
- [Controlnet Brightness / Illumination](https://huggingface.co/ioclab/ioc-controlnet/tree/main/models)

#### Face restoration

- CodeFormer
- GFPGAN
- Roop (Face swap)
  - [original project page](https://github.com/s0md3v/roop)
  - [AUTOMATIC1111 extension](https://github.com/s0md3v/sd-webui-roop)
- ReActor (Face swap)
  - [Stable Diffusion extension](https://github.com/Gourieff/sd-webui-reactor)

#### Upscaling

- Real-ESRGAN
  - [Model page](https://github.com/xinntao/Real-ESRGAN)
  - [Demo](https://huggingface.co/spaces/akhaliq/Real-ESRGAN)
- Latent upscalers
- [Swin2SR](https://huggingface.co/docs/transformers/model_doc/swin2sr)
- [OpenModelDB, a community-driven database of AI Upscaling models](https://openmodeldb.info/)

#### Animation

- Deforum
- AnimateDiff

## Tutorials

### Inpainting & outpainting

- [Stable Diffusion Art - inpainting](https://stable-diffusion-art.com/inpainting_basics/)
- [Stable Diffusion Art - outpainting](https://stable-diffusion-art.com/outpainting/)

### Upscaling

- [Stable Diffusion Art - AI upscaler](https://stable-diffusion-art.com/ai-upscaler/)
- [Stable Diffusion Art - ControlNet upscale](https://stable-diffusion-art.com/controlnet-upscale/)

### Animation

- [Stable Diffusion Art - text2video](https://stable-diffusion-art.com/text-to-video/)

### Embedding
- [Stable Diffusion Art - Embedding](https://stable-diffusion-art.com/embedding/)
