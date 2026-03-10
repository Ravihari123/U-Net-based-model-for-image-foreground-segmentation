# UNet Semantic Segmentation for Foreground Background Suppression

## Overview
This project implements a UNet-based convolutional neural network for semantic segmentation, specifically to segment human figures from grayscale images. It explores data preparation, model architecture variations, regularization techniques (e.g., data augmentation, dropout, early stopping), and performance evaluation on a dataset of 290 images with corresponding binary masks.
The work is conducted in Google Colab using TensorFlow and Keras, focusing on handling image datasets, building encoder-decoder models, and analyzing hyperparameters for improved generalization.

## Key Components
Dataset Curation: Loading images and masks from Google Drive, checking for corruption, resizing to 256x256, splitting into train/test sets, and visualization.
Model Building: Development of UNet architectures (encoder with convolutions/max-pooling, decoder with upsampling/transpose convolutions), compilation with Adam optimizer, and training with binary cross-entropy loss.
Regularization & Experiments: Incorporation of data augmentation (via ImageDataGenerator), early stopping, dropout layers, and learning rate adjustments to mitigate overfitting.
Evaluation: Assessment of model performance through accuracy, loss curves, and qualitative segmentation outputs.

## Tools & Libraries
Python 3 with TensorFlow/Keras for model building
NumPy, OpenCV for array operations and image processing
Matplotlib for visualizations
ImageDataGenerator for augmentation
Google Colab with GPU support

## Dataset
The project uses the Human Segmentation Dataset with 290 training images and corresponding masks.
Link: https://github.com/VikramShenoy97/Human-Segmentation-Dataset

## Main Learnings
UNet is effective for semantic segmentation tasks with limited data.
Data augmentation and early stopping significantly help in reducing overfitting.
Hyperparameter tuning (e.g., learning rate, dropout) is crucial for model convergence and performance.

## Results
1. Accuracy and Loss without augmentation and callback
   <image-card alt="Model" src="images/accuracy Without Augmentation And Callback.png" ></image-card>
2. Accuracy and Loss without early stopping
   <image-card alt="Model" src="images/accuracy Without Augmentation And Callback.png" ></image-card>
3. Accuracy and Loss with early stopping and data augmentation
   <image-card alt="Model" src="images/accuracy Without Augmentation And Callback.png" ></image-card>


