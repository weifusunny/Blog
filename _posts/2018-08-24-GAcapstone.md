---
layout: post
title: Capstone project at General Assembly
---


It is from Google landmark recognition challenge in www.kaggle.com. The goal of this challenge is to classify about 15k classes. Due to being a deep learning newcomer, I set the goal as to classify 5 classes in stead.

The outcome of my capstone project is that my deep learning model's classification accuracy for two classes is 96% and for five classes is 77%.

Here are the procedures of completing this project:

First of all, i did analyze the train and test data file and visualized some interesting findings. 

Secondly, i programmed a Python script file and ran the program to download 12000 images that are 1200 images for each of the top 10 most popular landmarks. 

Thirdly, i preprocessed all the images ready for feeding a deep learning model that targets at classifying images. 

Fourthly, i set up a simple convolutional neural network (CNN) model and a hybrid model (simple CNN plus pretrained RESNET50) separately.

Fifthly, i used the train images (500 or 1000 images per landmark) to train and validate the two models individually.

Due to the computer resource limitation and strict deadline, the model can fairly correctly classify up to five landmarks. However in the future the performance of the CNN model can be improved significantly. In other words, it will classify more classes with higher accuracy.
