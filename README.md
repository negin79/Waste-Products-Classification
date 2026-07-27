# Waste Classification Using Transfer Learning

This project develops a deep-learning image classifier that distinguishes between recyclable and organic waste. It demonstrates how transfer learning can be used to build an effective computer-vision model without training a convolutional neural network entirely from scratch.

A pre-trained VGG16 network is used as the feature extractor, followed by a custom classification head for binary waste classification. Two training strategies are explored:

1. Feature extraction with the VGG16 convolutional base frozen
2. Fine-tuning selected VGG16 layers to adapt the model to the waste dataset

The project includes image preprocessing and augmentation, model training, performance evaluation, visualization of training and validation curves, and predictions on previously unseen test images.

## Project Motivation

Manual waste sorting is time-consuming, labor-intensive, and susceptible to human error. Automated image classification could support more efficient sorting systems, reduce contamination of recyclable materials, and contribute to more sustainable waste-management processes.

## Key Features

- Binary classification of recyclable and organic waste
- Image preprocessing and data augmentation
- Transfer learning with a pre-trained VGG16 model
- Comparison of feature extraction and fine-tuning approaches
- Training and validation accuracy/loss visualization
- Evaluation on an independent test dataset
- Visualization of model predictions on test images

## Technologies

- Python
- TensorFlow
- Keras
- VGG16
- NumPy
- Matplotlib
- Jupyter Notebook

## Workflow

1. Load and preprocess the image dataset
2. Create training, validation, and test data generators
3. Load the VGG16 model with ImageNet weights
4. Train a custom classifier using frozen VGG16 features
5. Fine-tune selected layers of the pre-trained network
6. Compare the performance of both approaches
7. Evaluate the models and visualize sample predictions

## Results

The notebook compares the feature-extraction and fine-tuned models using training, validation, and test performance. Accuracy and loss curves are used to examine model convergence and identify possible overfitting.

> Add your final test accuracy, loss, and observations here after completing the experiments.

## Limitations and Future Improvements

The current model performs binary classification and is intended as a proof of concept. Future improvements could include:

- Classification of multiple waste categories
- Confusion matrix and class-specific performance metrics
- Testing on images from real-world environments
- Comparing VGG16 with more efficient architectures such as MobileNetV2
- Model explainability using Grad-CAM
- Deployment as a web or mobile application

## Acknowledgment

This repository is based on the final project of the Coursera/IBM course on deep learning with Keras and TensorFlow. The notebook was completed and documented as part of my practical study of transfer learning, fine-tuning, and image classification.
