# Image to Image

An input image and a text prompt are supplied as the input in image-to-image. The generated image will be conditioned by both the input image and text prompt. for example, using this amateur drawing and the prompt “photo of perfect green apple with stem, water droplets, dramatic lighting” as inputs, image-to-image can turn it into a professional drawing:

<br>
<figure>
  <img src="../../assets/lecture/andrew-wong-image-to-image-1.png" width="400px">
  <figcaption style="color:grey; font-style: italic;">Credit: Andrew Wong, 2023, "How does Stable Diffusion work?"</figcaption>
</figure>
<br>

## Process

**Step 1.** The input image is encoded to latent space.

<br>
<figure>
  <img src="../../assets/lecture/andrew-wong-image-to-image-2.png" width="400px">
  <figcaption style="color:grey; font-style: italic;">Credit: Andrew Wong, 2023, "How does Stable Diffusion work?"</figcaption>
</figure>
<br>

**Step 2.** Noise is added to the latent image. Denoising strength controls how much noise is added. If it is 0, no noise is added. If it is 1, the maximum amount of noise is added so that the latent image becomes a complete random tensor.

<br>
<figure>
  <img src="../../assets/lecture/andrew-wong-image-to-image-3.png" width="400px">
  <figcaption style="color:grey; font-style: italic;">Credit: Andrew Wong, 2023, "How does Stable Diffusion work?"</figcaption>
</figure>
<br>

**Step 3.** The noise predictor U-Net takes the latent noisy image and text prompt as input and predicts the noise in latent space (a 4x64x64 tensor).

<br>
<figure>
  <img src="../../assets/lecture/andrew-wong-image-to-image-4.png" width="400px">
  <figcaption style="color:grey; font-style: italic;">Credit: Andrew Wong, 2023, "How does Stable Diffusion work?"</figcaption>
</figure>
<br>

**Step 4.** Subtract the latent noise from the latent image. This becomes your new latent image.

<br>
<figure>
  <img src="../../assets/lecture/andrew-wong-image-to-image-5.webp" width="400px">
  <figcaption style="color:grey; font-style: italic;">Credit: Andrew Wong, 2023, "How does Stable Diffusion work?"</figcaption>
</figure>
<br>

**Steps 3 and 4** are repeated for a certain number of sampling steps, for example, 20 times.

**Step 5.** Finally, the decoder of VAE converts the latent image back to pixel space. This is the image you get after running image-to-image.

<br>
<figure>
  <img src="../../assets/lecture/andrew-wong-image-to-image-6.png" width="400px">
  <figcaption style="color:grey; font-style: italic;">Credit: Andrew Wong, 2023, "How does Stable Diffusion work?"</figcaption>
</figure>
<br>

So now you know what image-to-image is: All it does is to set the initial latent image with a bit of noise and a bit of input image. Setting denoising strength to 1 is equivalent to text-to-image because the initial latent image is entirely random noise.

## References

- [Andrew Wong, 2023, "How does Stable Diffusion work?", _Stable Diffusion Art_](https://stable-diffusion-art.com/how-stable-diffusion-work/)
