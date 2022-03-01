# U-Net-Cancer-Detection
### Detect brain tumors using the U-Net neural net architecture in TensorFlow

## Demo

<img width="735" alt="Screen Shot 2022-03-01 at 11 55 50 AM" src="https://user-images.githubusercontent.com/20956909/156223758-ece751ec-412d-4b59-809b-387a2437546b.png">

## How to train

1: Download the brain MRI dataset from Kaggle: https://www.kaggle.com/navoneel/brain-mri-images-for-brain-tumor-detection

2: Enter the dataset's top level directory

3: Run `python3 u_net_cancer_detection.py` or `U_Net_Cancer_Detection.pynb`

4: Once your weights file is generated, make sure to update line 280 with your weights file name: `model.load_weights('WEIGHT_FILE_NAME.h5')`
