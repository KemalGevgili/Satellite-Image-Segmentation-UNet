# Satellite Image Segmentation with UNet

This repository contains code for satellite image segmentation using the UNet architecture. The UNet model is trained to segment satellite images into different classes using annotated masks.

## Overview:

The repository contains Python code that utilizes PyTorch and torchvision libraries for deep learning-based image segmentation tasks. It includes:

- **Dataset Preparation**: Defines a custom dataset class `SatelliteDataset` for loading satellite images and their corresponding masks. Images and masks are loaded from specified directories and transformations are applied to augment the data.

- **Data Augmentation**: Utilizes various transformations such as random rotation, horizontal and vertical flips, and color jittering to augment the dataset. These transformations enhance the robustness of the model and help in better generalization.

- **Model Architecture**: Implements the UNet architecture using PyTorch. The UNet model consists of downsampling and upsampling paths with skip connections to capture both local and global features for accurate segmentation.

- **Training Loop**: Defines a training loop to train the UNet model on the prepared dataset. It uses the BCEWithLogitsLoss as the loss function and Adam optimizer for optimization.
