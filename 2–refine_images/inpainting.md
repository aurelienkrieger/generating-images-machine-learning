### Inpainting

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
