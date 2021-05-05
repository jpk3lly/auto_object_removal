![Pytests](https://github.com/mintusf/auto-object-removal/actions/workflows/pytest.yml/badge.svg?branch=main)

# auto-object-removal
An application to automatically remove selected objects from images.
It combines image segmentation with image inpainting to create automated pipeline to remove whole objects.
There are two removal modes:
* all instance removal (semantic segmentation is used)
* single instance removal (instance segmentation is used) (NOT YET IMPLEMENTED)

Implemented segmentation models:
* Deeplab (torchvision weigths used)

Used image inpainting models:
* CR fill ([this repository](https://github.com/zengxianyu/crfill))

The project is WIP.

# How to use

1. Setup and enter pipenv environment
```bash
pipenv sync
pipenv shell
```

2. Run the program
   1. Dash GUI
Dash GUI is implemented in the repository:

|  Image  | Video |
| ----------- | ----------- |
| ![](samples/GUI/GUI_1.PNG)      | ![](samples/GUI/GUI_gif.gif)       |
