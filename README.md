# Brain Tumor Detection using Convolutional Neural Networks

This repository contains code for a Convolutional Neural Network (CNN) model built with TensorFlow for detecting brain tumors from MRI images. The model is trained on a dataset containing brain MRI images categorized into two classes: normal and abnormal (indicating the presence of a tumor). It also includes functionality to clean the dataset by removing images with unknown or invalid extensions.

## Prerequisites

- Python 3.x
- TensorFlow
- OpenCV (cv2)
- NumPy
- Matplotlib

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/brain-tumor-detection.git
   cd brain-tumor-detection
   ```
2. Install dependencies:
   ```bash
   !pip install tensorflow tensorflow-gpu opencv-python matplotlib
   ```
## Model Architechture 

 The CNN model architecture consists of several Convolutional and MaxPooling layers followed by Dense    
 layers for classification. Below is a summary of the model:
 _________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d (Conv2D)              (None, 254, 254, 16)      448       
_________________________________________________________________
max_pooling2d (MaxPooling2D) (None, 127, 127, 16)      0         
_________________________________________________________________
conv2d_1 (Conv2D)            (None, 125, 125, 32)      4640      
_________________________________________________________________
max_pooling2d_1 (MaxPooling2 (None, 62, 62, 32)        0         
_________________________________________________________________
conv2d_2 (Conv2D)            (None, 60, 60, 16)        4624      
_________________________________________________________________
max_pooling2d_2 (MaxPooling2 (None, 30, 30, 16)        0         
_________________________________________________________________
flatten (Flatten)            (None, 14400)             0         
_________________________________________________________________
dense (Dense)                (None, 256)               3686656   
_________________________________________________________________
dense_1 (Dense)              (None, 1)                 257       
=================================================================
Total params: 3,696,625
Trainable params: 3,696,625
Non-trainable params: 0
_________________________________________________________________


 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.

