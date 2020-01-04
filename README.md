# Depth Estimation with Transfer Learning pretrained MobileNetV2


This project implements a deep learning neural network model to generate the depthe image of a given image.
Model is U-net model with MobileNetV2 as the encoder, and model has utilized skip connection from encoder to decoder.
Model generates a depth image of resolution 480x640 for the same sized input image.


## Getting Started

Model can be trained using the "train_mobilenetv2.ipynb".
 
In the file "Final Code.mat", you can find code for optimization using all the method such as ADMM, Proximal Point Algrithm and CVX.


Enter the values for the following varible before running the main program, default values are given in program:

Nopatient:             Number of patients

Nseg:                  Total number of training and testing segments for patients


##Data 
* [NYU Depth V2 (50K)](https://s3-eu-west-1.amazonaws.com/densedepth/nyu_data.zip) (4.1 GB): File is extraced in the "train_mobilenetv2.ipynb".

## Download a pretrained model 
*[Mobilenet](https://drive.google.com/drive/folders/1McNxDWmeWKgmJqD4cP_TW5IBdQPuSDMf)(55 MB)
### Results

A sample ECG signal segment:

![ECG image](https://github.com/alinstein/Human-Identification-with-ECG--/blob/master/observation/ecg.jpg)

Final sparse coefficient vector representation of the above ECG signal:

![Sparse coefficient](https://github.com/alinstein/Human-Identification-with-ECG--/blob/master/observation/maxpol2.jpg)
Following table shows the results obtained:

![Result image](https://github.com/alinstein/Human-Identification-with-ECG--/blob/master/Results.JPG)

## References

[1] J. Wang, M. She, S. Nahavandi and A. Kouzani, "Human Identification From ECG Signals Via Sparse Representation of Local Segments," in IEEE Signal Processing Letters, vol. 20, no. 10, pp. 937-940, Oct. 2013.
doi: 10.1109/LSP.2013.2267593
[2] W.-S. Lu, Course notes of Advanced Mathematical optimizations. 

## Authors

%Written by Alinstein Jose, University of Victoria.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details


