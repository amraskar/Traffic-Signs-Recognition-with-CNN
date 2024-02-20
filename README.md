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

**The architecture of the model is:**
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

Visual representation of the final model is given below.

![alt text](https://github.com/amraskar/Traffic-Signs-Recognition-with-CNN/blob/8b58bfdec02770c292a3111f50c94932bb253a24/model.png "Visual representation of the final model")

**Model accuracy:**
model got a 95% accuracy on the training dataset.
![alt text](https://github.com/amraskar/Traffic-Signs-Recognition-with-CNN/blob/8b58bfdec02770c292a3111f50c94932bb253a24/accuracy%20and%20loss%20curves.png "Graph for accuracy and the loss")

Testing the model with test dataset ==> I achieved a 95% accuracy in this model.

# The Final Result
Example 1:
Traffic sign name: Speed limit (50km/h)

![alt text](https://github.com/amraskar/Traffic-Signs-Recognition-with-CNN/blob/fc734962d72811625a4d6c9a43540ae2bf4c91db/Speed%20limit.png "Example 1")

Example 2:
Traffic sign name: Road work

![alt text](https://github.com/amraskar/Traffic-Signs-Recognition-with-CNN/blob/fc734962d72811625a4d6c9a43540ae2bf4c91db/Road%20work.png "Example 2")

Example 3:
Traffic sign name: Turn right ahead

![alt text](https://github.com/amraskar/Traffic-Signs-Recognition-with-CNN/blob/fc734962d72811625a4d6c9a43540ae2bf4c91db/Turn%20right%20ahead.png "Example 3")
