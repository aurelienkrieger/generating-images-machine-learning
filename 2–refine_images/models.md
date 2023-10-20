# Models

We can distinguish different types of models:

- Checkpoint models
- Fine-tuned models
- Models for advanced control

We are going to discuss these types of models in more details in the next chapters.

_Note: We can also mention Generative Adversarial Networks (GAN), which uses a different approach for generative AI than diffusion models._

<br>

The models can come in various file extensions:

- .ckpt
- .pt
- .safetensors
- Diffusers
- .bin

<br>

And in various formats:

- pruned
- full
- fp16
- fp32

## File extensions

- .pt

The original pytorch model format. It includes both the model architecture and the trained weights. This means that you have all the necessary information to continue training the model from where it left off, but they are larger in size. The downside of this format is that it is not secure. Someone can pack malicious codes in it. The code can run on your machine when you use the model.

- .ckpt

Checkpoint files primarily used for TensorFlow and PyTorch models. They also include both the model architecture and the trained weights, and are also insecure.

- .safetensors

Safetensors is an improved version of the .pt model format. It does the same thing as storing the weights but will not execute any codes. It is also faster.

- Diffusers

The most recent inovation. They are not a single file but a set of directories and files, each containing different aspect of the model. The advantage of this is that the models load from disk really fast. They also offer seamless integration with Hugging Face, a community-driven database of models, datasets, applications. Not all GUIs are compatbile with Diffusers yet.

## Formats

- pruned or EMA-only vs full

Pruned models focus on reducing the size and computational complexity of the model by removing certain weights, while EMA-Only models use a separate set of weights to improve model stability and generalization. These are separate techniques but generally speaking you can download them if you are only interested in using the model, not training it. This saves you disk space.

You will only need the full model if you want to fine-tune the model with additional training.

- fp16 vs fp32

FP stands for floating point. It is a computer’s way of storing decimal numbers. Here the decimal numbers are the model weights. FP16 takes 16 bits per number and is called half precision. FP32 takes 32 bits and is called full precision.

You rarely need a full-precision model though. The extra precision just stores noise. So, download the FP16 models if available. They are about half as big. This saves you disk space.

## Tutorials & resources

[Useful links & tutorials for Models](../resources/models.md)

## References

- [Andrew Wong, 2023, "Models", _Stable Diffusion Art_](https://stable-diffusion-art.com/models/)
- [InvokeAI, 2023, "Installing Models", _Github_](https://github.com/invoke-ai/InvokeAI/blob/main/docs/installation/050_INSTALLING_MODELS.md)
