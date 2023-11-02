# Inpainting

Inpainting is a process where we try to fill in parts of an image with new or tweaked content. In a technical sense, inpainting methods use the available information in an image (such as edges, textures, colors) to predict what the areas should look like, and then use the selected model to regenerate the image.

Inpainting is really just a particular case of image-to-image. Noise is added to the parts of the image you wanted to inpaint. The amount of noise is similarly controlled by denoising strength.

How Inpainting works is significantly impacted by the model you have selected. For best results, it is generally recommended to use an inpainting specific model; these are usually identified by the "-inpainting" term in the model name.

## Inpaiting in InvokeAI

On Invokes Unified Canvas, you can Inpaint by using the Brush (B) tool on the Mask layer to define an area that you would like to have regenerated. If you invoke with a masked area, the masked area will be inpainted on Invoking.

### Infill Method

Method to infill the selected area. Different methods function differently and will produce different result. The `patchmatch` seems to produce the best resultst in most cases.

### Scale Before Processing

Scales the selected area to the size best suited for the model before the image generation process. This can be used to increase the resolution of the bounded area to achieve finer details.

- Auto scales the bounded area’s width and height to the size best suited for the model used for inpainting
- None prevents any scaling from occurring before inpainting
- Manual allows the user to select the scaled width and height of the bounded area

### Workflow

- (optional) upscale the image before inpainting
- (optional) adjust the bounding box to focus on the part of the image you want to inpaint.
- (if adjusted bounding box). Keep in mind that the bounding box is all the model is aware of, so the prompt needs to be adjusted to adapt to the bounding box and only re-generate parts of the image you want to inpaint.
- adjust denoising scale. The higher, the more creative the AI will be. The lower, the closer it will stay to the original image
- (optional) use the brush tool to paint the base image and roughly define the shapes and colors you want to add / change
- use the brush tool to mask the area you want to inpaint
- select the infill methods
- (optional) increase the scale before processing for finer details
- repeat the process to mask any resulting seams between the new and base image to ensure that the generation fits in well

## Face Fixing in InvokeAI

As of InvokeAI, the easiest way to improve faces created during image generation is through the Inpainting functionality of the Unified Canvas. Simply add the image containing the faces that you would like to improve to the canvas, mask the face to be improved and run the invocation.

## Tutorials & resources

[Useful links & tutorials for Inpainting and Outpainting](../../resources/inpainting_outpainting.md)

## References

- [InvokeAI, 2023, "Postprocessing", _Github_](https://github.com/invoke-ai/InvokeAI/blob/main/docs/features/POSTPROCESS.md)
- [Andrew Wong, 2023, "How does Stable Diffusion work?", _Stable Diffusion Art_](https://stable-diffusion-art.com/how-stable-diffusion-work/)
