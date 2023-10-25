# Fine-tuned models

## What is fine-tuning?

Fine-tuning is a common technique in machine learning. It takes a model that is trained on a wide dataset and trains a bit more on a narrow dataset.

A fine-tuned model tends to generate images similar to those used in the training. For example, the Anything v3 model is trained with anime images. It generates anime-style images by default.

## Why do people make Stable Diffusion models?

The Stable diffusion base model is great but is not good at everything. For instance it could be difficult to generate images of a specific genre of anime. Instead of tinkering with the prompt, you can use a custom model that is fine-tuned with images of that sub-genre.

There are different ways to make a fine-tuned model. We will discuss these techniques in more details in the section [4 - Model Training 💾](../4-model_training/README.md). What is important to know, is that they all start from a checkpoint model.

## Tutorials & resources

[Useful links & tutorials for Models](../resources/models.md). Includes a selection of fine-tuned models with download links.

## References

- [Andrew Wong, 2023, "Models", _Stable Diffusion Art_](https://stable-diffusion-art.com/models/)
