# Portraits

## 1. Generate base image

- prompt
- sd_xl_base_1.0_0.9vae model
- 2:3 aspect ratio
- sd_xl_refiner_1.0 (late start, 0.8)
- DPM++ 2S Karras

## 2. Adjust details

- face restoration
  - brush as mask on face

- adjust details (eg. chair)
  - brush as base on chair
    - pick color
    - adjust transparency
  - brush as mask over painted area

- add details
  - brush as base
    - pick color
    - no transparency
  - brush as mask over painted area

- limb restoration

- seam
  - brush as mask on seam

## 3. Adjust composition

- use Photoshop / Gimp to take best elements and create final composition
- use Image to Image for final generation
