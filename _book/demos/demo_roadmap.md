# Demos roadmap

# 1 – Enter the Latent Space 🚀

## Person reading a book

- models
  - SD1.5 base checkpoint model for text to image

- workflow
  - write first basic prompt
  - use style qualifiers
  - optional: use negative prompt

- learnings
  - how to best describe a subject in a prompt
  - learn about basic parameters

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

- workflow
  - use basic prompt "Portrait of person as nature magic celestial"
  - use negative prompts to change the style
  - introduce universal negative prompt

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


## CLIP, prompt generators, boilerplates

- workflow
  - look at different online resources

- learnings
  - have an overview on prompt resources

## Prompt craft challenge (from InvokeAI Discord)

- workflow
  - post a AI-generated image
  - participants submit a prompt that should generate images that are identical
  - when the submission period ends, we generate images for each prompt submitted
  - all images will be posted for voting. No prompts or metadata will be included - so participants don't know which one is theirs

- learnings
  - practice and improve prompting techniques


# 2 – Refine images 🎨

## Fine-tuned models

- models
  - Various SD1.5 trained models for text to image
    - Juggernaut
    - OpenJourney
    - Fantasy and Art by Zovya
    - Realistic Vision
  - SDXL base checkpoint model for text to image

- workflow
  - use previous prompts with other models
  - remove negative prompt
  - compare results with various models

- learnings
  - how to import custom models
  - how to improve the general aesthetics with custom models
  - discuss limitations of trained models
  - models depend on their training set
  - each model have optimal resolutions

## Photo editing: "please remove the person behind"

- models
  - SD1.5 inpaint model for image to image

- workflow
  - use input picture of a wedding couple with "a person behind"
  - use inpainting to remove the person behind

- learnings
  - how to use inpainting for photo editing (remove elements)


## Add elements to a landscape

- models
  - SD1.5 base checkpoint model for text to image
  - SD1.5 inpaint model for image to image

- workflow
  - use advanced prompt "beautiful landscape"
  - use brush to guide diffusion process
  - use inpainting to add new elements to the image

- learnings
  - how to use inpainting for new content on existing images
  - how to use bounding box and resolution parameters
  - use smaller generation steps for better results

## Grandma with a biker's jacket

- models
  - SD1.5 base checkpoint model for text to image
  - SD1.5 inpaint model for image to image

- workflow
  - use advanced prompt "head and shoulders portrait"
  - use inpainting to restore the face
  - use Inpaint Replace to modify completly the image

- learnings
  - how to use inpainting for image correction
  - use smaller generation steps for better results

## Greek scolar with a laptop

- models
  - SD1.5 base checkpoint model for text to image
  - SD1.5 inpaint model for image to image

- workflow
  - use advanced prompt "greek scholar in library"
  - use inpainting to change book to laptop

- learnings
  - how to use inpainting for image correction
  - use smaller generation steps for better results


## Face restoration of a portrait

- models
  - SD1.5 base checkpoint model for text to image
  - SD1.5 inpaint model for image to image

- workflow
  - use advanced prompt "head and shoulders portrait"
  - use inpainting to restore the face

- learnings
  - how to use inpainting for image correction (face restoration)
  - how to use bounding box and resolution parameters
  - use smaller generation steps for better results

## Apply colors / Hair

- models
  - SD1.5 base checkpoint model for text to image
  - SD1.5 inpaint model for image to image

- workflow
  - use advanced prompt "portrait"
  - use brush to guide diffusion process
  - use inpainting to change the colour of his/her hair

- learnings
  - how to use inpainting for image correction (coloration)
  - how to use bounding box and resolution parameters
  - use smaller generation steps for better results

## Apply colors / Outfit

- models
  - SD1.5 base checkpoint model for text to image
  - SD1.5 inpaint model for image to image

- workflow
  - use advanced prompt "wizard"
  - use brush to guide diffusion process
  - use inpainting to change the colour of his/her outfit

- learnings
  - how to use inpainting for image correction (coloration)
  - use smaller generation steps for better results


## Extended landscape

- models
  - SD1.5 base checkpoint model for text to image
  - SD1.5 inpaint model for image to image

- workflow
  - use advanced prompt "beautiful landscape"
  - use outpainting to extend the image
  - use upscaling
  - use inpainting to add details to the image

- learnings
  - how to use outpainting for to extend existing images
  - how to use upscaling for higher resolutions
  - how to use inpainting for image correction (details)


# 3 – Image Compositing 📐


## Darth Vader in the bus

- models
  - SD1.5 trained model for text to image

- workflow
  - use basic image to image for style transfer
  - start from image of person in the bus
  - adapt to being Darth Vader

- learnings
  - how to use image to image for style transfer

## _In the style of_

- models
  - SD1.5 trained model for text to image

- workflow
  - use basic image to image for style transfer
  - start from image of person in the bus
  - adapt to being Darth Vader

- learnings
  - how to use image to image for style transfer

## "Breaking Bad but in Japan" (credit: [Demon Flying Fox](https://www.instagram.com/p/CyEUX9dtUBT/?hl=en))

- models
  - SD1.5 trained model for text to image

- workflow
  - use basic image to image for style transfer
  - start from image of person in the bus
  - adapt to being Darth Vader

- learnings
  - how to use image to image for style transfer


## Darth Vader dancing

- models
  - SD1.5 trained model for text to image
  - ControlNet OpenPose

- workflow
  - use ControlNet OpenPose for advanced image to image
  - start from image of person dancing
  - adapt to being Darth Vader dancing

- learnings
  - how to use ControlNet OpenPose


## French village

- models
  - SD1.5 trained model for text to image
  - ControlNet Depth

- workflow
  - use ControlNet Depth for advanced image to image
  - start from image of Tokyo streets
  - prompt "French village" that follows the same perspective
  - play with parameters for more control over composition

- learnings
  - how to use ControlNet Depth for perspective


## Darth Vader in a landscape

- models
  - SD1.5 trained model for text to image
  - ControlNet OpenPose
  - ControlNet Depth

- workflow
  - use ControlNet OpenPose from image of person sitting
  - use ControlNet Depth from image of landscape
  - prompt to generate image of Darth Vader using the two ControlNet

- learnings
  - how to use a combinaison of various ControlNet models


## Beautiful drawing

- models
  - SD1.5 trained model for text to image
  - ControlNet

- workflow
  - make basic drawing
  - use ControlNet to detect edges
  - use text to image to generate professional drawing
  - use small generation steps for better results

- learnings
  - how to make profesional drawings from basic sketches


## Beautiful photoshoping

- models
  - SD1.5 trained model for text to image
  - ControlNet

- workflow
  - make basic photoshoping
  - use text to image to generate professional image
  - use small generation steps for better results

- learnings
  - how to make profesional images from basic photoshoping


# 4 - Model Training 💾

## Embedding for style modification

- models
  - SD1.5 base checkpoint model for text to image
  - EasyNegative

- workflow
  - use basic prompt "Portrait of person as nature magic celestial"
  - use negative prompts to change the style
  - introduce universal negative prompt
  - introduce embedding

- learnings
  - how to use embedding to modify the style of an image

## Embedding for new styles

- models
  - SD1.5 base checkpoint model for text to image
  - Atompunk Style

- workflow
  - use basic prompts using embedding Atompunk Style

- learnings
  - how to use embedding to create a new style

## Embedding for new objects

- models
  - SD1.5 trained model for text to image
  - Embedding with specific object

- workflow
  - use basic prompt
  - use embedding to introduce the object in the generated image

- learnings
  - how to use embedding to introduce new objects

## Embedding for new concepts

- models
  - SD1.5 trained model for text to image
  - Clutter Home

- workflow
  - use basic prompt "interior of a gallery"
  - use embedding to change the composition

- learnings
  - how to use embedding to introduce new concepts
  - how to use embedding to modify the composition of an image


## IP Adapter for style modification

- models
  - SD1.5 trained model for text to image
  - IP Adapter

- workflow
  - use basic prompt "robot"
  - use the generated image as input for IP Adapter
  - use prompt to generate images inspired by the robot

- learnings
  - how to use IP Adapter to modify the style of a generated image


## IP Adapter for new objects

- models
  - SD1.5 trained model for text to image
  - IP Adapter

- workflow
  - use prompt "robot"
  - use IP Adapter to generate variations of the robot
  - use IP Adapter + prompt "trash can" to generate a trash can version of the robot

- learnings
  - how to use IP Adapter to introduce new objects

## IP Adapter for image variations

- models
  - SD1.5 trained model for text to image
  - IP Adapter

- workflow
  - use prompt "clouds"
  - use IP Adapter to generate variations of the cloud
  - alternative: feed IP Adapter with images from a certain style / artist

- learnings
  - how to use IP Adapter to introduce new objects
  - how to use IP Adapter to generate variations of an image
  - how to use IP Adapter to generate variations of an artistic style

## IP Adapter for consitent portraits

- models
  - SD1.5 trained model for text to image
  - IP Adapter

- workflow
  - use prompt "person"
  - use IP Adapter to generate variations of that person

- learnings
  - how to use IP Adapter to generate variations of a concept or object

## LoRA for new styles

- models
  - SD1.5 base checkpoint model for text to image
  - Atompunk Style

- workflow
  - use basic prompts using embedding Atompunk Style

- learnings
  - how to use embedding to create a new style

## LoRA for new concepts

- models
  - SD1.5 trained model for text to image
  - LoRA for action poses

- workflow
  - use basic prompt
  - use LoRA generate images in the action pose

- learnings
  - how to use LoRA to introduce new concepts

## LoRA for consistent portraits

- models
  - SD1.5 trained model for text to image
  - LoRA trained on a specific person

- workflow
  - use basic prompt
  - use LoRA to generate variations of that person

- learnings
  - how to use LoRA to generate variations of an object

## Train your models

- workflow
  - use embedding to introduce a new object
  - use LoRA to introduce a new object


# 5 – Extra tips & Animations 🎥

## Monster QR code

- models
  - SD1.5 trained model for text to image
  - ControlNet Monster QR Code

- workflow
  - use QR code as input for image to image for ControlNet
  - use prompt to generate "readable" QR-images

- learnings
  - how ControlNet can be used to control specific aspect of an image

## Outgrown garden (credit: [Fred Huergo](https://www.instagram.com/p/CH0jk3KHrhC/))

- models
  - SD1.5 trained model for text to image
  - ControlNet Monster QR Code

- workflow
  - use symmetric image as input for image to image for ControlNet
  - use prompt to generate an image of a garden following the symmetry of the input image

- learnings
  - how ControlNet can be used to control specific aspect of an image

## Image composition in the style of Giuseppe Arcimboldo

- models
  - SD1.5 trained model for text to image
  - ControlNet

- workflow
  - use image of a face as input for image to image
  - use prompt of "cup of fruits" to make a portrait in the style of artist Giuseppe Arcimboldo
  - use small generation steps for better results
  - alternative : use text to show hidden message

- learnings
  - how to use ControlNet for optical illusions

## ControlNet OpenPose

- models
  - SD1.5 trained model for text to image
  - OpenPose Face
  - OpenPose Face only
  - OpenPose Hand

- workflow
  - use and compare various ControlNet OpenPose

- learnings
  - have an overview on the OpenPose models

## Other ControlNet processors

- models
  - SD1.5 trained model for text to image
  - ControlNet Canny
  - ControlNet Line Art

- workflow
  - use and compare various ControlNet OpenPose

- learnings
  - have an overview on the OpenPose models

## Self-loop AI

- models
  - SD1.5 trained model for text to image
    - OpenJourney
    - Juggernaut

- workflow
  - generate image from OpenJourney (or use MidJourney image) - [tutorial](https://www.youtube.com/watch?v=TrcwBSlczfQ)
  - use as input for image to image with prompt to generate photorealistic images

- learnings
  - how to use AI images as input for general composition & intricate details

## Abstract images with ControlNet

- models
  - SD1.5 trained model for text to image
  - ControlNet OpenPose
  - ControlNet Depth

- workflow
  - use image as input for image to image with anoother image as input for ControlNet + prompt to generate more abstract images
  - make image ship
  - use image with random colours and shapes as input for image to image
  - use ship image as input for ControlNet + prompt

- learnings
  - how ControlNet can be used to control specific aspect of an image
  - how it can be associated with basic image to image

## Frame interpolation

- models
  - SD1.5 trained model for text to image
  - AnimateDiff

- workflow
  - use AnimateDiff to animate a still generated image

- learnings
  - how to use AnimateDiff

## Deforum

- models
  - SD1.5 trained model for text to image
  - Deforum

- workflow
  - use Deforum for Text to Video

- learnings
  - how to do Text to Video

## Gif to Gif

- models
  - SD1.5 trained model for text to image
  - Gif to Gif model

- workflow
  - use Gif to Gif model for style transfer

- learnings
  - how to use Gif to Gif model for style transfer

## Morphing

- models
  - SD1.5 trained model for text to image
  - Morphing model

- workflow
  - use a morphing model to create an animation from two generated images

- learnings
  - how to use a morphing model to create an animation from two generated images

# 6 – Final Presentations ✨











--------



# Ideas

- colorize B&W image
- regional prompting
- inclusive portraits (sliders: weight, age, muscles, gender, skin tone)
- consistent face
- limb restoration
- Instruct Pix2Pix´
- Use IP adapter to inspire the impaiting or outpainting
