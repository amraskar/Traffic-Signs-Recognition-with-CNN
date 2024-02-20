# Traffic Signs Recognition: Project Overview
* The objective of the project is to apply the concepts of a CNN and build a working model to recognize the traffic signs.
* I implemented a deep neural network model that can classify traffic signs present in the image into different categories.

# Code and Resources Used 
**Python Version:** 3.11  
**Packages:** os, PIL, numpy, pandas, matplotlib, seaborn, scikit-learn, tensorflow, keras

# Dataset Used
I used the public dataset available at Kaggle: https://www.kaggle.com/datasets/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign

# Defining the CNN model
I used the Keras Model from Sequential API.

## The architecture of the model is:
* 2 Conv2D layer (filter=32, kernel_size=(5,5), activation=”relu”)
* MaxPool2D layer ( pool_size=(2,2))
* Dropout layer (rate=0.25)
* 2 Conv2D layer (filter=64, kernel_size=(3,3), activation=”relu”)
* MaxPool2D layer ( pool_size=(2,2))
* Dropout layer (rate=0.25)
* Flatten layer to squeeze the layers into 1 dimension
* Dense Fully connected layer (256 nodes, activation=”relu”)
* Dropout layer (rate=0.5)
* Dense layer (43 nodes, activation=”softmax”)
