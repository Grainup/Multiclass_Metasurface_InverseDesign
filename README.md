# Multiclass_Metasurface_InverseDesign


## Introduction
Welcome to the Raman Lab GitHub! This repo will walk you through the code used in the following publication: ___

Here, we use a conditional deep convolutional generative adversarial network (cDCGAN) to inverse design across multiple classes of metasurfaces.

## Requirements
The following software is required to run the provided scripts. As of this writing, the versions below have been tested and verified. Training on GPU is recommended due to lengthy training times with GANs. 

-Pytorch 1.9.0

-CUDA 10.2 (Recommended for training on GPU)

Installation instructions for Pytorch (with CUDA) is at: https://pytorch.org/

## Steps
### 1) Train the cDCGAN (DCGAN.py)
Download the files in the 'Training Data' folder and update the following lines in the 'DCGAN.py' file:
```python
## Define File Locations (Images, Spectra, and CNN Model Save)
img_path = 'C:/.../*.png'
spectra_path = 'C:/.../Spectra.csv'
save_dir = 'C:/.../model.h5'
```
Running this file will train the cDCGAN and save the model in the specified location. Depending on the available hardware, the training process can take up to a few hours.
