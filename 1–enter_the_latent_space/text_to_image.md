## Text to Image

Now you know all the inner mechanics of Stable Diffusion, let’s go through some examples of what happens under the hood.

In text-to-image, you give Stable Diffusion a text prompt, and it returns an image.

Step 1. Stable Diffusion generates a random tensor in the latent space. You control this tensor by setting the seed of the random number generator. If you set the seed to a certain value, you will always get the same random tensor. This is your image in latent space. But it is all noise for now.

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-92.png" width="400px">


Step 2. The noise predictor U-Net takes the latent noisy image and text prompt as input and predicts the noise, also in latent space (a 4x64x64 tensor).

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-94.png" width="400px">

Step 3. Subtract the latent noise from the latent image. This becomes your new latent image.

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-95.png" width="400px">

Steps 2 and 3 are repeated for a certain number of sampling steps, for example, 20 times.

Step 4. Finally, the decoder of VAE converts the latent image back to pixel space. This is the image you get after running Stable Diffusion.

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-96-1024x602.png" width="400px">

## References

- [Andrew Wong, 2023, "How does Stable Diffusion work?", _Stable Diffusion Art_](https://stable-diffusion-art.com/how-stable-diffusion-work/)
