# Chest X-Ray Classification for COVID-19 and Pneumonia Detection

## Overview
This project aims to classify chest X-ray images into three categories: 
1. **Normal**
2. **COVID-19**
3. **Pneumonia** 

The classification model is built using Convolutional Neural Networks (CNN) in TensorFlow and Keras. The dataset used is the **Chest X-ray Images (COVID-19)** dataset, which consists of labeled chest X-ray images from patients diagnosed with COVID-19, pneumonia, and healthy individuals.

The main objective is to create a model that can distinguish between these three classes based on chest X-ray images.

## Dataset
The dataset used for training and testing is publicly available and can be accessed [here](https://www.kaggle.com/datasets/prashant268/chest-xray-covid19-pneumonia). It consists of images placed in the following folders:
- **train/**: Contains training images
- **test/**: Contains testing images

The images are categorized into subdirectories: **NORMAL**, **COVID19**, and **PNEUMONIA**.

## Code Walkthrough
### 1. Dataset Summary
The code first walks through the dataset and provides a summary of the directories and image counts.

### 2. Image Preprocessing
The image paths are obtained, and labels are generated based on the directory names (NORMAL, COVID19, PNEUMONIA). The images are then converted into a DataFrame for further processing.

### 3. Data Augmentation
Using Keras' `ImageDataGenerator`, data augmentation techniques are applied to the training images to improve model generalization.

### 4. CNN Model
A simple Convolutional Neural Network (CNN) is built using Keras. The model consists of three convolutional layers followed by max-pooling layers. The model is compiled with the Adam optimizer and categorical crossentropy loss function.

### 5. Model Training
The model is trained for 10 epochs on the training data and evaluated on the test data. The test accuracy score achieved by the model is **0.845**.

## Results
The model achieved a test accuracy score of **0.845** after training for 10 epochs, which shows that the model is able to classify the chest X-rays into the three categories with reasonable performance.
