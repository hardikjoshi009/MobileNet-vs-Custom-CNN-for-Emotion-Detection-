# MobileNet vs Custom CNN for Emotion Detection

This project implements an emotion detection model using PyTorch, focusing on comparing the performance of MobileNet and a custom CNN architecture on the FER 2013 dataset. The goal is to analyze the differences in accuracy, model complexity, and inference time between the two approaches.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Model Architectures](#model-architectures)
- [Results](#results)
- [Conclusion](#conclusion)

## Overview

Emotion detection from facial expressions is a significant challenge in the field of computer vision. This project explores two distinct approaches: leveraging the pre-trained MobileNet architecture and a custom-built CNN model. The aim is to assess their effectiveness in accurately classifying emotions and to provide insights into their respective efficiencies.

## Features

- **Pre-trained MobileNet**: Utilizes transfer learning to achieve better performance with fewer resources.
- **Custom CNN**: A simple convolutional neural network designed from scratch for comparison.
- **Performance Metrics**: Validation accuracy, model complexity, and inference time.
- **Visualization**: Includes visualizations of training and validation loss and accuracy.

## Dataset

The FER 2013 dataset consists of 48x48 pixel grayscale images representing different facial expressions across various emotions. The dataset contains the following classes:
- Angry
- Disgust
- Fear
- Happy
- Sad
- Surprise
- Neutral

## Model Architectures

### MobileNet

- **Architecture**: MobileNet is designed for mobile and edge devices, featuring depthwise separable convolutions to reduce the model size and complexity while maintaining accuracy.
- **Validation Accuracy**: 67.78%

### Custom CNN

- **Architecture**: A custom convolutional neural network with several convolutional layers, pooling layers, and fully connected layers tailored for emotion detection.
- **Validation Accuracy**: 29.99%

## Results

The comparison yielded the following insights:

- **MobileNet**:
  - Validation Accuracy: 67.78%
  - Model Complexity: Low (efficient for deployment)
  - Inference Time: Faster due to optimized architecture

- **Custom CNN**:
  - Validation Accuracy: 29.99%
  - Model Complexity: Higher (requires more tuning)
  - Inference Time: Slower compared to MobileNet

## Conclusion

The results demonstrate that MobileNet significantly outperforms the custom CNN in both accuracy and efficiency for the task of emotion detection. This analysis emphasizes the advantages of using pre-trained models in practical applications, particularly when computational resources are a concern.
