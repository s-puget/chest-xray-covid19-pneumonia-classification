# Chest X-Ray Classification: COVID-19 & Pneumonia Detection

## Overview

This project implements **Deep Learning** to classify chest X-ray images into three categories: **Normal, COVID-19, and Pneumonia**. We first train a **CNN from scratch** and then improve performance using **Transfer Learning with VGG16**.

## Dataset

The dataset is sourced from Kaggle:  
[Chest X-Ray: COVID-19 & Pneumonia](https://www.kaggle.com/datasets/prashant268/chest-xray-covid19-pneumonia)  

It contains X-ray images labeled as:
- **NORMAL** (Healthy lungs)
- **COVID19** (Lungs affected by COVID-19)
- **PNEUMONIA** (Lungs affected by other pneumonia types)

## Models Implemented

### 1. CNN (Trained from Scratch)
- **Architecture**: 3 convolutional layers, max pooling, dense layers.
- **Test Accuracy**: **92.3%**
- **Limitations**: Longer training time, potential overfitting.

### 2. Transfer Learning (VGG16)
- **Pre-trained VGG16** model used for feature extraction.
- **Custom classifier** added on top with dense layers.
- **Test Accuracy**: **94.5%**
  
## Results & Comparison

| Model        | Epochs | Test Accuracy |
|-------------|--------------|--------------|
| CNN (Scratch) | 10       | 92.3%       |
| VGG16 (Transfer Learning) | 5 | 94.5% |

### Visualizations:
- **Accuracy & Loss Plots**: To track model performance.
- **Confusion Matrix**: To evaluate misclassifications.

## References

- Kaggle Dataset: [Chest X-Ray: COVID-19 & Pneumonia](https://www.kaggle.com/datasets/prashant268/chest-xray-covid19-pneumonia)
