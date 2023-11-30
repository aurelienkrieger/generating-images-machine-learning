# LoRA (Low-Rank Adaptation)

While Dreambooth trains an entire new model by updating the model’s weights, LoRA takes a different approach: it adds microscopic new weights to the model instead. The method was originally developed for LLMs (Large Language Models like GPT-4), but works well for txt2img models like Stable Diffusion as well. A LoRA is typically in the hundreds of MB range, so somewhere between a Textual Inversion and a Dreambooth checkpoint.

## How to use it

Like a Textual Inversion, LoRAs have a trigger word. To add a LoRA with weight, use the following syntax in the prompt or the negative prompt:

`<lora: name: weight>`

`name` is the name of the LoRA model. It can be different from the filename. <br>
`weight` is the emphasis applied to the LoRA model. It is similar to a keyword weight. The default is 1. Setting it to 0 disables the model.

## References

- [The beginner's guide to fine-tuning Stable Diffusion](https://octoml.ai/blog/the-beginners-guide-to-fine-tuning-stable-diffusion/), 2023, Justin Gage
- [What are LoRA models and how to use them in AUTOMATIC1111](https://stable-diffusion-art.com/lora/), Andrew Wong, 2023, _Stable Diffusion Art_
