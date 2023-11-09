# Seed

During the first step of a Text to Image process, Stable Diffusion generates a random tensor in the latent space. You control this tensor by setting the seed of the random number generator. If you set the seed to a certain value, you will always get the same random tensor.

## Reproducibility vs Exploration

It is best to change one thing at a time so you know what is working and what isn't. Sometimes you just need to try a new image, and other times using a new prompt might be the ticket. Setting a random seed will generate a new random image for each batch, so it can be used for exploration. You can also consider turning off the “random” Seed - Using the same seed with the same settings will produce the same image, which makes it the perfect way to learn exactly what your changes are doing and ensure reproducibility.

## Interpolation

AUTOMATIC1111 offer the option to control the degree of interpolation to produce a transition between the images genearted by two seeds. See [Andrew Wong, 2023, "Stable Diffusion WebUI AUTOMATIC1111: A Beginner’s Guide"](https://stable-diffusion-art.com/automatic1111/#Extra_seed_options) for more details.

# Resources

- [Know these Important Parameters for stunning AI images](https://stable-diffusion-art.com/know-these-important-parameters-for-stunning-ai-images), Andrew Wong, 2023, _Stable Diffusion Art_
- [Getting Started with AI Image Generation](https://invoke-ai.github.io/InvokeAI/help/gettingStartedWithAI/), InvokeAI
