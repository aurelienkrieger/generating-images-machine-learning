# Model training

## Key techniques & models

- Improved VAE
- Additional training
- Merging models
- Embedding (result of [Textual Inversion](https://textual-inversion.github.io/))
- IP Adapter
- LoRA (Low-Rank Adaptation)
  - LyCORIS (Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion)
  - LoHa (LoRA with Hadamard Product representation)
  - LoCon (Conventional LoRA)
- Dreambooth
- Hypernetworks

## Improved VAE

VAE stands for variational autoencoder. It is part of the neural network model that encodes and decodes the images to and from the smaller latent space, so that computation can be faster. When people say downloading and using a VAE, they refer to using an improved version of it. This happens when the model trainer further fine-tunes the VAE part of the model with additional data. Instead of releasing a whole new model, which is a big file, they release only the tiny part that has been updated.

## Tutorials & resources

[Useful links & tutorials for Models](../resources/model_training.md)

## References

- [Andrew Wong, 2023, "Models", _Stable Diffusion Art_](https://stable-diffusion-art.com/models/)
- [Andrew Wong, 2023, "How to use VAE to improve eyes and faces", _Stable Diffusion Art_](https://stable-diffusion-art.com/how-to-use-vae/)
