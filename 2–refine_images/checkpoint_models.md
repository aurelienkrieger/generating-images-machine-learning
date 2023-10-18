# Checkpoint models

## Stable Diffusion v1 vs v2

### Model difference

Stable Diffusion v2 uses OpenClip for text embedding. Stable Diffusion v1 uses Open AI’s CLIP ViT-L/14 for text embedding. The reasons for this change are

- OpenClip is up five times larger. A larger text encoder model improves image quality.
- Although Open AI’s CLIP models are open-source, the models were trained with proprietary data. Switching to the OpenClip model gives researchers more transparency in studying and optimizing the model. It is better for long-term development.

### Training data difference

Stable Diffusion v1.4 is trained with

- 237k steps at resolution 256×256 on laion2B-en dataset.
- 194k steps at resolution 512×512 on laion-high-resolution.
- 225k steps at 512×512 on “laion-aesthetics v2 5+“, with 10% dropping of text conditioning.

Stable Diffusion v2 is trained with

- 550k steps at the resolution 256x256 on a subset of LAION-5B filtered for explicit pornographic material, using the LAION-NSFW classifier with punsafe=0.1 and an aesthetic score >= 4.5.
- 850k steps at the resolution 512x512 on the same dataset on images with resolution >= 512x512.
- 150k steps using a v-objective on the same dataset.
- Resumed for another 140k steps on 768x768 images.

Stable Diffusion v2.1 is fine-tuned on v2.0
- additional 55k steps on the same dataset (with punsafe=0.1)
- another 155k extra steps with punsafe=0.98

So basically, they turned off the NSFW filter in the last training steps.

### Outcome difference

Users generally find it harder to use Stable Diffusion v2 to control styles and generate celebrities. Although Stability AI did not explicitly filter out artist and celebrity names, their effects are much weaker in v2. This is likely due to the difference in training data. Open AI’s proprietary data may have more artwork and celebrity photos. Their data is probably highly filtered so that everything and everyone looks fine and pretty.

The v2 and v2.1 models are not popular. People use the fine-tuned v1 model exclusively. But this is going to change with the release of the SDXL model.

## SDXL model

The SDXL model is the official upgrade to the v1 and v2 models. The model is released as open-source software.

It is a much larger model. In the AI world, we can expect it to be better. The total number of parameters of the SDXL model is 6.6 billion, compared with 0.98 billion for the v1.5 model.

<img src="https://stable-diffusion-art.com/wp-content/uploads/2023/07/image-26.png" width="400px">

The SDXL model is, in practice, two models. You run the base model, followed by the refiner model. The base model sets the global composition. The refiner model adds finer details.

You can run the base model alone without the refiner.

The changes in the SDXL base model are:

- The text encoder combines the largest OpenClip model (ViT-G/14) and OpenAI’s proprietary CLIP ViT-L. It is a smart choice because it makes SDXL easy to prompt while remaining the powerful and trainable OpenClip.
- New image size conditioning that aims to use training images smaller than 256×256. This significantly increases the training data by not discarding 39% of the images.
- The U-Net is three times larger than v1.5.
- The default image size is 1024×1024. This is 4 times larger than the v1.5 model’s 512×512. (See image sizes to use with the SDXL model)

## References

- [Andrew Wong, 2023, "How does Stable Diffusion work?", _Stable Diffusion Art_](https://stable-diffusion-art.com/how-stable-diffusion-work/)
