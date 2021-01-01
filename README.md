# Traffic-Sign-Analyzer

This is a console application that aim to detect the **traffic signs** encountered in camera. <br>
This project is built using keras and openCV libraries.

### Introduction

This is a Convolutional neural network based approach over traditional model. This system approaches the problem by employing 3 layered neural network and passing the preprocessed images in them through pipeline. 

### What to expect?

The model should detect and process the traffic signs of 43 different classes. <br>
It should return the class and name of the input (traffic sign) provided.


### Project Setup

Images are 32 (width) x 32 (height) x 3 (RGB color channels).<br>
Training set is composed of 22271 images.<br>
Validation set is composed of 5568 images.<br>
Test set is composed of 6960 images. <br>
There are 43 classes (e.g. Speed Limit 20km/h, No entry, Bumpy road, etc.). <br>

![Screenshot 2021-01-01 175255](https://user-images.githubusercontent.com/66209332/103440011-28d09480-4c68-11eb-8064-0bc3f604bbd3.jpg) <br>
Exploratory Visualization of Images

### No. of Images of each class

A difference can be observed in the no. of different classes of images, this change in number also results in different accuracy of each class.

![image](https://user-images.githubusercontent.com/66209332/103440113-08eda080-4c69-11eb-98a0-4a3139b28f96.png)

### Preprocessing stage 

![Screenshot 2021-01-01 193816](https://user-images.githubusercontent.com/66209332/103440300-51598e00-4c6a-11eb-84ec-78187adb75d9.jpg)

### Architecture

Network has 3 Convolutional Layers – kernel size: 3 X 3
Activation function – ReLU (followed by 2 X 2 maxPooling operation)
Last 3 layers are connected producing 43 classes (using SoftMax activation fn.)

![image](https://user-images.githubusercontent.com/66209332/103440125-1c990700-4c69-11eb-985b-1cef2b06340a.png)

![image](https://user-images.githubusercontent.com/66209332/103440478-0d678880-4c6c-11eb-8635-acd45e4c9052.png)

### Observations
![image](https://user-images.githubusercontent.com/66209332/103440133-2a4e8c80-4c69-11eb-8a82-ac8271d6cf40.png)
![image](https://user-images.githubusercontent.com/66209332/103440139-30446d80-4c69-11eb-9730-877302414702.png)

It is observed that after 8 epochs the loss and accuracy becomes constant and the result is 99% accurate.


