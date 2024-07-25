# CatDogClassifier

This repository contains an image classification model that differentiates between cats and dogs. It includes all necessary scripts for data preprocessing, model training, evaluation, and deployment. The project leverages deep learning techniques to achieve high accuracy in identifying pet images.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Data Preprocessing](#data-preprocessing)
- [Training](#training)
- [Requirements](#requirements)
- [Inference](#inference)
- [Results](#results)
- [Contributing](#contributing)

## Installation

To get started, clone the repository and install the required dependencies:

```bash
git clone https://github.com/yourusername/CatDogClassifier.git
cd CatDogClassifier
pip install -r requirements.txt

Usage
Data Preparation: Place your cat and dog images in the following directory structure:
cats_and_dogs/
├── train/
│   ├── cats/
│   └── dogs/
├── validation/
│   ├── cats/
│   └── dogs/
└── test/
    ├── cats/
    └── dogs/

Model Architecture
The model uses transfer learning with the VGG16 architecture, followed by a GlobalAveragePooling layer and two dense layers.

Data Preprocessing
The dataset is augmented using the ImageDataGenerator class from TensorFlow to improve the model's generalization.

Training
The model is trained using the Adam optimizer and binary cross-entropy loss. Early stopping and learning rate reduction callbacks are used to prevent overfitting.

Requirements
tensorflow
matplotlib
numpy

Inference
After training, the model weights are saved. If the weights file is present, the model loads the weights and performs inference on the test set, displaying the predictions.

Results
The model's accuracy and loss during training and validation are plotted and displayed.

Contributing
Contributions are welcome! Please submit a pull request or open an issue to discuss any changes.

