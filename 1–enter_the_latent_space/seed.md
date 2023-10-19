# Seed

During the first step of a Text to Image process, Stable Diffusion generates a random tensor in the latent space. You control this tensor by setting the seed of the random number generator. If you set the seed to a certain value, you will always get the same random tensor.

## Reproducibility

If you use the same seed with the same prompt, model and parameters, you will get the exact same image, so it can be used to ensaure the reproducibility.

## Exploration

Setting a random seed will generate a new random image for each batch, so it can be used for exploration.

# Resources

- [Andrew Wong, 2023, "Know these Important Parameters for stunning AI images", _Stable Diffusion Art_](https://stable-diffusion-art.com/know-these-important-parameters-for-stunning-ai-images/#Seed)
