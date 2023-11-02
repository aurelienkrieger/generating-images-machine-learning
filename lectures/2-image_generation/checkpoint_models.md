# Checkpoint models

## Introduction

Stable Diffusion Models, sometimes called checkpoint models, are pre-trained models for generating a particular style of images. They are the real Stable Diffusion models. They contain all you need to generate an image. No additional files are required. They are large, typically 2 – 7 GB.

What kind of images a model generates depends on the training images. A model won’t be able to generate a cat’s image if there’s never a cat in the training data. Likewise, if you only train a model with cat images, it will only generate cats.

## Stable Diffusion Base Models

### v1 vs v2 models

Currently the most popular SD model is v1.5. StabilityAI later released a v2 and v2.1 models but these models are not popular. People use the fine-tuned v1 model exclusively.

### SDXL model

On July 2023, StabilityAI release the SDXL model, its latest iteration of text-to-image generation models. They state it is an improvement in many ways:
- The default image size is 1024×1024. This is 4 times larger than the v1.5 model’s 512×512. (See image sizes to use with the SDXL model)
- High quality in virtually any art style, including photorealism
- More intelligent with simpler language (soon the end of prompt engineering)
- Much larger model. The total number of parameters of the SDXL model is 6.6 billion, compared with 0.98 billion for the v1.5 model
- Fine-tuning and advanced control

<img src="https://stable-diffusion-art.com/wp-content/uploads/2023/07/image-26.png" width="400px">

The SDXL model is, in practice, two models. You run the base model, followed by the refiner model. The base model sets the global composition. The refiner model adds finer details. You can run the base model alone without the refiner.

In facts though, people tend to be a bit disappointed by this new release, the main reasons being:
- it is much slower and consumes more VRAM, which makes it less accessible for people with slower machines and less energy efficient
- the quality leap is not that high, compared to fine-tuned v1.5 models which already give great results
- some of the advanced control that was anounced is not quite there yet. SD1.5 has still better support for outpainting and other advanced control models

But this may change, it takes times for the community to find out how to best fine-tune a new model and develop all the "utility" models for advanced control.

## Other models

### DALL-E 3 model

On October 2023, OpenAI has released the latest iteration of its text-to-image generate model, Dall-E. They also announced that it understands significantly more nuance and detail than their previous systems. Something to keep an eye on.

## Tutorials & resources

[Useful links & tutorials for Models](../../resources/models.md). Includes download links.

## References

- [Andrew Wong, 2023, "How does Stable Diffusion work?", _Stable Diffusion Art_](https://stable-diffusion-art.com/how-stable-diffusion-work/)
- [Andrew Wong, 2023, "Models", _Stable Diffusion Art_](https://stable-diffusion-art.com/models/)
- [StabilityAI, 2023, "Announcing SDXL 1.0"](https://stability.ai/blog/stable-diffusion-sdxl-1-announcement)
- [OpenAI, 2023, "DALL-E 3"](https://openai.com/dall-e-3)
