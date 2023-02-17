# Pneumonia Image Classification with Deep Learning

This project aims to classify chest x-ray images as either normal or showing signs of pneumonia using deep learning techniques.


## <b>Table of Contents</b>
Introduction <br>
Dataset<br>
Methods<br>
Dependencies <br>



## <b> Introduction </b>
Pneumonia is a common and serious respiratory infection that can be life-threatening, especially for vulnerable populations such as the elderly, infants, and people with weakened immune systems. Chest x-ray images are commonly used to diagnose pneumonia, but manual interpretation by radiologists can be time-consuming and error-prone. In this project, we aim to develop a deep learning model that can accurately classify chest x-ray images as either normal or showing signs of pneumonia.


## <b> Dataset </b>
We used the Chest X-Ray Images dataset from Kaggle, which contains 5,856 chest x-ray images labeled as either normal or pneumonia. The dataset is split into three sets: training, validation, and test, with 5,216, 16,610, and 624 images, respectively.

You can download the dataset from https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia. Please refer to the Kaggle website for the terms and conditions of use.

## <b> Methods </b>
For this project, we used a convolutional neural network (CNN) to classify chest x-ray images as either normal or pneumonia. Our CNN architecture consists of the following layers:

1. Conv2D layer with 32 filters, a kernel size of (2,2), and ReLU activation function
2. MaxPooling2D layer
3. Conv2D layer with 64 filters, a kernel size of (2,2), and ReLU activation function
4. MaxPooling2D layer
5. Conv2D layer with 128 filters, a kernel size of (2,2), and ReLU activation function
6. MaxPooling2D layer
7. Dense layer with 512 units and ReLU activation function
8. Dense layer with 1 unit and sigmoid activation function

We trained the network using binary cross-entropy loss and the Adam optimizer.

You can modify the architecture of the network by adjusting the number of filters, kernel sizes, and activation functions of the layers to improve performance or reduce computational complexity.






## <b> Dependencies </b>
The project was developed using Python 3.7 and the following dependencies:

tensorflow==2.4.0 <br>
keras==2.4.3 <br>
numpy==1.19.4 <br>
opencv-python==4.4.0.46<br>
matplotlib==3.3.3