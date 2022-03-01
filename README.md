# U-Net-Cancer-Detection
### Detect brain tumors using the U-Net neural net architecture in TensorFlow

## What is U-Net

* U-Net is a neural network architecture for image segmentation. 

* U-Net paper: https://arxiv.org/pdf/1505.04597.pdf

* <img width="642" alt="Screen Shot 2022-03-01 at 12 11 43 PM" src="https://user-images.githubusercontent.com/20956909/156225238-4379060e-ed88-4a21-9875-3c8c80493778.png">

* U-Net consistes of a contracting path (encoder), and expansive path (decoder). This compression forces the network to isolate and remember only the most important features from the image. The expansive path outputs a sigmoid probability for each pixel (0-1), where pixel values > 0.5 are considered to be a tumor.
* Feature maps from the contracting path are concatenated with feature maps in the expansive stage to preserve fine grain details from the image.

## Demo

<img width="735" alt="Screen Shot 2022-03-01 at 11 55 50 AM" src="https://user-images.githubusercontent.com/20956909/156223758-ece751ec-412d-4b59-809b-387a2437546b.png">

## How to train

1: Download the brain MRI dataset from Kaggle: https://www.kaggle.com/navoneel/brain-mri-images-for-brain-tumor-detection

2: Enter the dataset's top level directory

3: Run `python3 u_net_cancer_detection.py` or `U_Net_Cancer_Detection.pynb`

4: Once your weights file is generated, make sure to update line 280 with your weights file name: `model.load_weights('WEIGHT_FILE_NAME.h5')`
