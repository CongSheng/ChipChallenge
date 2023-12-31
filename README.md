# ChipChallenge
Chip's Challenge involves using Intel's OpenVino in creating and implementing 
AI on Intel's devices.

## Installation
First, Intel's OpenVINO and YOLOv8 have to be downloaded by following the 
instructions on https://www.intel.com/content/www/us/en/developer/tools/openvino-toolkit/download.html?ENVIRONMENT=DEV_TOOLS&OP_SYSTEM=WINDOWS&VERSION=v_2023_0&DISTRIBUTION=PIP.
As PyTorch is my preferred library, the version can be installed via the
following code:
```
pip install openvino-dev[pytorch]==2023.0.0
```
Other than this, the other packages can be installed via pip or conda, with the
lists shown in `requirements.txt`.

## Beginner Challenge
The beginner challenge requires participants to just use the OpenVINO YOLOv8 
notebook to detect any object. As such, the notebook was first downloaded from
https://github.com/openvinotoolkit/openvino_notebooks/tree/main/notebooks/230-yolov8-optimization.
There are many interesting notebooks present there as well, including stable 
diffusion voice conversion, quantization-aware training and etc.

The YOLOv8 notebook requires the use of `nccf` and `onnx`, and the packages can
be downloaded simply by running the notebook. Alternatively, the packages can 
be downloaded through pip install in the terminal. 

After which, running through the notebook is a breeze. Just to further try out 
the optimized YOLOv8 model, I ran through my own videos of some cats.

<img src="https://github.com/CongSheng/ChipChallenge/blob/d3f80374e65c0a50f80f2f0e7d17ad5a457d9acd/images/cat_as_cat.png" width="400" alt="Adorable cat">
<center>Fig 1: Running object detection on a video of me interacting with a cat.</center>

<img src="https://github.com/CongSheng/ChipChallenge/blob/b53de9131fb555c4c361d34bcf671b48f49df802/images/cat_as_bear.PNG" width="400" alt="Cat classified as bear - Failed example">
<center>Fig 2: At the same time, one has to admit that even SOTA classifier has its bad days.</center>