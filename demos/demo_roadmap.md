# Demos roadmap

# 1 – Enter the Latent Space

## Person reading a book

- models
  - SD1.5 base checkpoint model for text to image

- workflow
  - write first basic prompt
  - use style qualifiers
  - optional: use negative prompt

- learnings
  - how to best describe a subject in a prompt
  - introduce parameters

## Paris in a rainy day, without people

- models
  - SD1.5 base checkpoint model for text to image

- workflow
  - use basic prompt "Paris in a rainy day"
  - use negative prompt to remove "people"
  - use keyword weights to emphasis negative prompt

- learnings
  - how to use negative prompt to remove things
  - how to use keyword weights

## Person in the stars, not windy, not immature

- models
  - SD1.5 base checkpoint model for text to image

- workflow
  - use basic prompt "Portrait of person as nature magic celestial"
  - use negative prompt to make hair go down
  - use negative prompt to make person older

- learnings
  - how to use negative prompt to modify the image

## Person in the stars, with different styles

- models
  - SD1.5 base checkpoint model for text to image
  - EasyNegative

- workflow
  - use basic prompt "Portrait of person as nature magic celestial"
  - use negative prompts to change the style
  - introduce universal negative prompt
  - introduce embedding

- learnings
  - how to use negative prompt to modify the style of an image

## English breakfast

- models
  - SD1.5 base checkpoint model for text to image

- workflow
  - use basic prompt "English breakfast"
  - use keyword weights to change composition of the plate

- learnings
  - how to use keyword weights


## Famous person

- models
  - SD1.5 base checkpoint model for text to image

- workflow
  - use basic prompt for the portrait of a famous person
  - use keyword blends to mix with other famous person

- learnings
  - how to use keyword blends


## Person reading a book (custom model)

- models
  - SDXL base checkpoint model for text to image
  - SD1.5 trained models for text to image
    - Juggernaut
    - OpenJourney
    - Fantasy and Art by Zovya
    - Realistic Vision

- workflow
  - use same first basic prompt
  - remove negative prompt
  - compare results with various models

- learnings
  - models depend on their training set
  - each model have optimal resolutions


# Ideas

- Face restoration
- use AI generated images (eg. from MidJourney) as input for img2img + prompt to generate photorealistic images
- use image as input for img2img + other image as input for controlnet + prompt to generate more asbtract images
- img2img, use smaller generation steps for better results
- [change hair color with inpainting](https://civitai.com/models/46422?modelVersionId=129549)
- [use Ip adapters](https://www.youtube.com/watch?v=hFBJwYTCvHg) for the style
- use Ip adapters for consistent face
- use other techniques for consistent face
- CLIP interrogator
- regional prompting ?
- demo prompt generators & boilerplates
- make inclusive portraits

## Prompt craft challenge (InvokeAI Discord)

The rules are simple.

-------

1️⃣  - Each week, I'll post an image in ⁠🏆promptcraft-challenges

2️⃣  - After deep consideration and tinkering, you'll submit a prompt (not an image). The prompt should reliably generate images that are identical (or as close as you can!) to the image posted.

3️⃣  - When the submission period ends, @The Invoker will generate images for each prompt submitted, using the settings detailed in the prompt. For the sake of RNG, four images will be generated - All four will be shared, so consistency is a key element your peers will be voting on.

4️⃣ - All images will be posted for voting. No prompts or metadata will be included - So you won't know which one is yours!

5️⃣ - Once the votes are tallied, a winner will be crowned Promptcrafter - They'll get a big boost to their invocation rank, and their prompt may be included (in full or in part) in future versions of InvokeAI!

We'll share all of the prompts (including the winner's) at the conclusion of the challenge!
