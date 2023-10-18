#  What is Stable Diffusion?

In the simplest form, Stable Diffusion is a text-to-image model. Give it a text prompt. It will return an AI image matching the text.

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-77.png" width="400px">

Stable Diffusion belongs to a class of deep learning models called diffusion models. They are generative models, meaning they are designed to generate new data similar to what they have seen in training. In the case of Stable Diffusion, the data are images.

## Forward diffusion

A forward diffusion process adds noise to a training image, gradually turning it into an uncharacteristic noise image. The forward process will turn any cat or dog image into a noise image. Eventually, you won’t be able to tell whether they are initially a dog or a cat.

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-81.png" width="400px">

## Reverse diffusion

What if we can reverse the diffusion? Like playing a video backward. Going backward in time. Starting from a noisy, meaningless image, reverse diffusion recovers a cat.

## Stable Diffusion model training

To reverse the diffusion, we need to know how much noise is added to an image. The answer is teaching a neural network model to predict the noise added. It is called the noise predictor in Stable Diffusion. It is a U-Net model. The training goes as follows.

1. Pick a training image, like a photo of a cat.
2. Generate a random noise image.
3. Corrupt the training image by adding this noisy image up to a certain number of steps.
4. Teach the noise predictor to tell us how much noise was added. This is done by tuning its weights and showing it the correct answer.

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-82.png" width="400px">

Noise is sequentially added at each step. The noise predictor estimates the total noise added up to each step. After training, we have a noise predictor capable of estimating the noise added to an image.

## Reverse diffusion

Now we have the noise predictor. How to use it?

We first generate a completely random image and ask the noise predictor to tell us the noise. We then subtract this estimated noise from the original image. Repeat this process a few times. You will get an image of a cat.

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-84.png" width="400px">

For now, image generation is unconditioned. We will see how to apply conditioning to have control over the image generated.

## Differences between diffusion models and latent diffusion models

The above diffusion process is in image space. It is computationally very, very slow because the image space is enormous. For instance, a 512×512 image with three color channels (red, green, and blue) is a 786,432-dimensional space. Diffusion models like Google’s Imagen and Open AI’s DALL-E are in pixel space. They have used some tricks to make the model faster but still not enough.

Stable Diffusion, on the other hand, is a latent diffusion model which is designed to solve the speed problem. Instead of operating in the high-dimensional image space, it first compresses the image into the latent space. The latent space is 48 times smaller so it reaps the benefit of crunching a lot fewer numbers. That’s why it’s a lot faster.

## Variational Autoencoder

It is done using a technique called the variational autoencoder. The Variational Autoencoder (VAE) neural network has two parts: (1) an encoder and (2) a decoder. The encoder compresses an image to a lower dimensional representation in the latent space. The decoder restores the image from the latent space.

<img src="https://stable-diffusion-art.com/wp-content/uploads/2022/12/image-85.png" width="400px">

The latent space of Stable Diffusion model is 4x64x64, 48 times smaller than the image pixel space. All the forward and reverse diffusions we talked about are actually done in the latent space.

The VAE decoder is also responsible for recovering fine details that may have been lost by the encoder. By further fine-tuning the VAE decoder, the model can paint finer details.

## Image resolution

The image resolution is reflected in the size of the latent image tensor. The size of the latent image is 4x64x64 for 512×512 images only. It is 4x96x64 for a 768×512 portrait image. That’s why it takes longer and more VRAM to generate a larger image.

Since Stable Diffusion v1 is fine-tuned on 512×512 images, generating images larger than 512×512 could result in duplicate objects, e.g., the infamous two heads. The SDXL model has a larger default size of 1,024 x 1,024 pixels.

## Reverse diffusion in latent space

Here’s how latent reverse diffusion in Stable Diffusion works.

1. A random latent space matrix is generated.
2. The noise predictor estimates the noise of the latent matrix.
3. The estimated noise is then subtracted from the latent matrix.
4. Steps 2 and 3 are repeated up to specific sampling steps.
5. The decoder of VAE converts the latent matrix to the final image.

## References

- [Andrew Wong, 2023, "How does Stable Diffusion work?", _Stable Diffusion Art_](https://stable-diffusion-art.com/how-stable-diffusion-work/)
