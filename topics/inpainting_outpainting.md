# Inpainting / Outpainting

## Inpainting

### Tutorials

- [InvokeAI tutorial](https://www.youtube.com/watch?v=kzRL88ffv1o)
- [Stable Diffusion Art tutorial for AUTOMATIC1111](https://stable-diffusion-art.com/inpainting-remove-extra-limbs/)
- [Monzon Media tutorial](https://www.youtube.com/watch?v=aU0jGZpDIVc)

### Parameters

- (optional) upscale image
- (optional) adjust bounding box
- (if adjusted bounding box) adjust prompt to bounding box
- use the same model that generates the image
- adjust denoising scale
- use brush in base or mask
- (optional) use refiner
- infill methods
  - patchmatch ([installation guide](https://invoke-ai.github.io/InvokeAI/installation/060_INSTALL_PATCHMATCH/))
  - cv2
  - tile
  - lama
- (optional) increase scale before processing

## Outpainting

### Tutorials

- [Stable Diffusion Art tutorial for AUTOMATIC1111](https://stable-diffusion-art.com/outpainting/)
- SDXL: outpainting not optimal ([Reddit conversation](https://www.reddit.com/r/invokeai/comments/16jhb8f/comment/k19ydow/))
- SD1.5: more adjusted for outpainting

### Parameters

- use the same model that generates the image
