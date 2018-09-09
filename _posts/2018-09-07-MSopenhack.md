---
layout: post
title: Microsoft's Machine Learning OpenHack
---

As a fresh data science graduate (graduated from General Assembly in Aug.2018), luckily I attended OpenHack Machine Learning event organised by Microsoft in Sydney from 4th to 6th of September.

There are about 15 groups and 4-5 people in each group. There are six challenges.

First of all, to set up a VM (virtual machine with Linux at Microsoft Azure) for data science workspace while setting you may choose number of CPUs, disk size and so on.

Secondly to download the dataset (about 2000 image files of 12 classes) , preprocess the images to the format required and split them to train and test set.

For the third step, to build one or multiple machine learning model(s) to train the train dataset and display the test results including accuracy and confusion matrix. KNN turned out to be the best model and the accuracy is about 89%.

For the fourth one, deep learning model (CNN) was deployed to classify the 12 classes. My capstone project at GA was building a CNN plus RESNET50 model to classify landmarks (https://www.kaggle.com/c/landmark-recognition-challenge) and surprisingly my capstone experience helped me to contribute to this challenge. My group achieved 95% accuracy by deploying a simple CNN model that consists of only two convolutional layers, one maxpooling layer and one or two drop-out, flatten and dense layer(s).

The fifth challenge is to deploy the model as a real-time webservice on Azure and the sixth one is to utilize a modern model like Faster R-CNN to detect and create a bounding box around the detected object from the images in a designated website and their URLs are supplied.

The OpenHack event is still going on (for another one week) and participants will access Microsoft Azure to complete the challenges. This was a great experience and I learned a lot about Microsoft Azure and Linux command, setting up VM, API in the cloud (Azure machine learning CLI standalone).

I know I just started my exciting journey and adventure in data science as OpenHack event has just given me more tools to explore the fascinating AI world.
