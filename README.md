# Depth Estimation with Transfer Learning pretrained MobileNetV2


This project implements a deep learning neural network model to generate the depth image of a given image.
Model is a U-net model with MobileNetV2 as the encoder, and model has utilized skip connection from encoder to decoder.
Model generates a depth image of resolution 480x640 for input image of same size.

![Results](https://github.com/alinstein/Depth_estimation/blob/master/CombineGIF.gif)


This project was implemented taking reference from the following paper: 

[High Quality Monocular Depth Estimation via Transfer Learning (arXiv 2018)](https://arxiv.org/abs/1812.11941)
**[Ibraheem Alhashim]** and **Peter Wonka**

## Getting Started

##### Model is trained using the IPYTHON file "train_mobilenetv2.ipynb".

* Download the dataset and give the location of dataset.
* Change the following according to the needs: batch_size, epochs, lr (learning rate).
Load the pretrained model if needed.
 
##### IPYTHON file "test_img.ipynb" can be used to generate the depth image on pretrained model.

* Give the location for the dictionary of images to be converted and load the pretrained model

##### IPYTHON file "test_video.ipynb" can be used to generate the depth video on pretrained model.

* Give the location for the dictionary of images to be converted and load the pretrained model.

#### Implementation of the Depth estimation using Densenet model is in the folder "Densenet_depth_model".


## Dataset 
* [NYU Depth V2 (50K)](https://s3-eu-west-1.amazonaws.com/densedepth/nyu_data.zip) (4.1 GB): File is extraced while running the "train_mobilenetv2.ipynb".

## Download the pretrained model 
* [Mobilenet](https://drive.google.com/drive/folders/1rDvtiwUgYbhzk8ZPdQ176abv-u6SaZzI?usp=sharing) (55 MB). Pretrained model is trained on 2 NVIDIA GeForce GTX 1080 for 6 hours(6 epoches). 

## Author

Written by Alinstein Jose, University of Victoria.

