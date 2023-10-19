# Sketch to image

## Tutorials

- [InvokeAI tutorial](https://www.youtube.com/watch?v=kzRL88ffv1o)
- [Patrick Galbraith tutorial](https://www.youtube.com/watch?v=-JR5vLc1T8c)

## Models / Extensions

- [Composable diffusion for AUTOMATIC1111](https://github.com/ashen-sensored/stable-diffusion-webui-two-shot)
- [Regional prompter for AUTOMATIC1111](https://github.com/hako-mikan/sd-webui-regional-prompter)

## 1. Sketch base image

- fill canvas with plain colour and draw image
- or : import sketch as image

## 2. Generate
- use ControlNet to catch general structure
- generate image with high denoising strenght (better: iterate multiple times with lower denoising strength)

## 3. Fine-tune

- inpainting
- photo montage
- eraser
