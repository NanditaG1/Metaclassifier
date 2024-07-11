# Lung Cancer Detection using Metalearning Approach

## Overview
This project presents a novel metalearning-based framework for the detection and classification of lung cancer tissues using deep learning techniques. The method leverages the strengths of multiple pretrained convolutional neural network (CNN) models to achieve high accuracy in detecting and classifying common types of lung cancer tissues: Benign tissue, Squamous Cell Carcinoma, and Adenocarcinoma.

## Motivation
Lung cancer is a dangerous disease with varying treatment plans based on the types and location of cancerous cells. Early detection is crucial for effective treatment and improving survival rates. Traditional manual examination of chest CT scans is challenging and prone to misdiagnoses. This project aims to enhance detection accuracy using a metalearning-based approach.

## Features
- Combination of features from InceptionResNetV1, EfficientNetB7, and DenseNet121 pretrained CNN models.
- Application of dimensionality reduction techniques on fused features.
- Use of Support Vector Machine (SVM) as the metaclassifier.
- High classification accuracy of 99.43%.
- Quantitative analysis through classification accuracy and confusion matrix computation.

## Dataset
The experiments have been conducted on a publicly available benchmark dataset for lung histopathological images. The dataset includes images of different lung tissue types used to train and validate the model.

## Methodology
1. **Feature Extraction**: Extract features from the penultimate layer (global average pooling) of InceptionResNetV1, EfficientNetB7, and DenseNet121 models.
2. **Feature Fusion**: Fuse the extracted features to create a comprehensive feature set.
3. **Dimensionality Reduction**: Apply dimensionality reduction to the fused features.
4. **Classification**: Use the SVM classifier on the reduced feature set for final classification.

## Results
The proposed method achieves a classification accuracy of 99.43%, outperforming existing state-of-the-art methods. The effectiveness of the approach is validated through comprehensive quantitative analysis, including classification accuracy and confusion matrix computation.

## Installation
To run this project, you'll need to install the following dependencies:
```bash
pip install tensorflow scikit-learn numpy pandas
