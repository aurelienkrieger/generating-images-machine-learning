# Depth to Image

Depth-to-image is an enhancement to image-to-image; it generates new images with additional conditioning using a depth map.

Step 1. The input image is encoded into the latent state

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-101.png" width="400px">

Step 2. An AI depth model estimates the depth map from the input image.

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-102.png" width="400px">

_list of depth models_

Step 3. Noise is added to the latent image. Denoising strength controls how much noise is added. If the denoising strength is 0, no noise is added. If the denoising strength is 1, the maximum noise is added so that the latent image becomes a random tensor.

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-100.png" width ="400px">

Step 4. The noise predictor estimates the noise of the latent space, conditioned by the text prompt and the depth map.

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-103.png" width="400px">

Step 5. Subtract the latent noise from the latent image. This becomes your new latent image.

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-95.png" width="400px">

Steps 4 and 5 are repeated for the number of sampling steps.

Step 6. The decoder of VAE decodes the latent image. Now you get the final image from depth-to-image.

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-104.png" width="400px">

## References

- [Andrew Wong, 2023, "How does Stable Diffusion work?", _Stable Diffusion Art_](https://stable-diffusion-art.com/how-stable-diffusion-work/)
