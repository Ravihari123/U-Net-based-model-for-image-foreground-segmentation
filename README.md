# UNet Semantic Segmentation for Foreground Background Suppression

## Overview
This project implements a U-Net based model for foreground segmentation and background suppression, developed as part of the Comp-5421 Deep Learning course assignment. The goal is to separate human figures (foreground) from the background in portrait images using semantic segmentation techniques. The model is built using TensorFlow and Keras in Google Colab.

Key features:
- Dataset curation including loading, corruption checks, and splitting.
- U-Net model with convolutional layers, batch normalization, dropout, and upsampling.
- Experiments with attribute and model regularization.
- Evaluation through performance metrics and visualizations.

The project uses the Human Segmentation Dataset with 290 training images and corresponding masks.
Link: https://github.com/VikramShenoy97/Human-Segmentation-Dataset

## Model Architecture
The U-Net model is designed for pixel-level segmentation. It includes an encoder for feature extraction (convolutions, max pooling) and a decoder for upsampling with skip connections to preserve spatial details. Layers used: Conv2D, MaxPool2D, Dropout, BatchNormalization, UpSampling2D, Conv2DTranspose. Optimizer: Adam. Loss: Binary Cross-Entropy.
