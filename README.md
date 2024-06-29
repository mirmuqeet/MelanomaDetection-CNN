# Melanoma Detection using Convolutional Neural Networks

This repository contains an assignment to build a Convolutional Neural Network (CNN) based multiclass classification model to accurately detect melanoma, a deadly form of skin cancer, along with other types of skin diseases. This project uses TensorFlow for model building and training.

## Problem Statement

Melanoma accounts for 75% of skin cancer deaths and early detection is crucial. This project aims to develop a solution that can evaluate images and alert dermatologists about the presence of melanoma, thereby reducing the manual effort needed in diagnosis.

## Dataset

The dataset consists of 2,357 images of various skin conditions, including:

- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

Images are sourced from the International Skin Imaging Collaboration (ISIC).

## Project Pipeline

1. **Data Reading/Understanding**
   - Define the path for training and testing images.

2. **Dataset Creation**
   - Create, train, and validate the dataset with a batch size of 32.
   - Resize images to 180x180 pixels.

3. **Dataset Visualization**
   - Visualize one instance of all nine classes in the dataset.

4. **Model Building and Training**
   - Create a CNN model to detect the nine classes.
   - Rescale images to normalize pixel values between (0,1).
   - Choose an appropriate optimizer and loss function.
   - Train the model for ~20 epochs.
   - Check for evidence of overfitting or underfitting.

5. **Resolving Underfitting/Overfitting**
   - Apply data augmentation strategies.

6. **Model Building and Training on Augmented Data**
   - Create and train the model on augmented data.
   - Train for ~20 epochs.
   - Check if the earlier issues are resolved.

7. **Class Distribution Examination**
   - Identify classes with the least and most samples.
   - Handle class imbalances using the augmentor library.

8. **Model Building and Training on Rectified Class Imbalance Data**
   - Create and train the model on rectified data.
   - Train for ~30 epochs.
   - Evaluate if issues are resolved.

## Results and Findings

- Detailed findings from each training phase.
- Analysis of model performance and steps taken to address overfitting/underfitting.
- Strategies used for handling class imbalance and their effectiveness.
