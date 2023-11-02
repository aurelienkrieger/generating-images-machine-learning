# Image resolution

## VRAM

VRAM (video RAM) is dedicated computer memory specifically used to store image data for a computer display. VRAM's purpose is to ensure the smooth execution of graphics display.

The image resolution you choose for your generated image is reflected in the size of the latent image tensor. Since the size of the latent image is 4x64x64 for 512×512 images, it is 4x96x64 for a 768×512 portrait image. That’s why it takes longer and more VRAM to generate a larger image.

## Optimal resolutions

Since Stable Diffusion v1 is fine-tuned on 512×512 images, generating images larger than 512×512 could result in duplicate objects, e.g., the infamous two heads. To generate a larger image, keep at least one side of the image to 512 pixels and then use an AI upscaler or image-to-image function for image upscaling. See the chapter [Upscaling](../3-refine_images/upscaling.md) for more details.

The SDXL model has a larger default size of 1,024 x 1,024 pixels.

Also, the image ratio may affect the composition of an image. For instance, we would have better chance to achieve a full body portrait by choosing a portrait ratio like 2:3.

## References

- [Alexander S. Gillis, 2021, "VRAM (video RAM)", _TechTarget_](https://www.techtarget.com/searchstorage/definition/video-RAM)
