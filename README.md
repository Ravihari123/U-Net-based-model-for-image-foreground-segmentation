# UNet Semantic Segmentation for Foreground Background Suppression

## Overview
This project implements a U-Net based model for foreground segmentation and background suppression, developed as part of the Comp-5421 Deep Learning course assignment. The goal is to separate human figures (foreground) from the background in portrait images using semantic segmentation techniques. The model is built using TensorFlow and Keras in Google Colab.
Key features:

Dataset curation including loading, corruption checks, and splitting.
U-Net model with convolutional layers, batch normalization, dropout, and upsampling.
Experiments with attribute and model regularization.
Evaluation through performance metrics and visualizations.

The project uses the Supervisely Persons dataset (or similar portrait images) with 290 training images and corresponding masks.
