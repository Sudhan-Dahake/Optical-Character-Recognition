# Optical Character Recognition

This project implements a custom neural network from scratch using only NumPy and pure mathematics. The model is trained on the MNIST dataset and achieves an accuracy of 88.8%.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Usage](#usage)
- [Results](#results)


## Introduction

Optical Character Recognition (OCR) is a technology used to convert different types of documents, such as scanned paper documents, PDFs, or images taken by a digital camera, into editable and searchable data. This project demonstrates a basic OCR system using a custom neural network to recognize handwritten digits from the MNIST dataset.

## Dataset

The MNIST dataset is a large database of handwritten digits commonly used for training various image processing systems. Each image is a 28x28 grayscale image, and the dataset contains 60,000 training images and 10,000 test images.

## Model Architecture

The neural network consists of the following layers:
- **Input Layer**: 784 neurons (28x28 pixels)
- **Hidden Layer**: 10 neurons
- **Output Layer**: 10 neurons (corresponding to digits 0-9)

Activation functions used:
- **ReLU** (Rectified Linear Unit) for the hidden layer
- **Softmax** for the output layer

## Training

The model is trained using gradient descent. The loss function used is categorical cross-entropy. The training process involves the following steps:
1. **Initialization**: Randomly initialize the weights and biases.
2. **Forward Propagation**: Compute the activations for each layer.
3. **Backward Propagation**: Compute the gradients of the loss with respect to the weights and biases.
4. **Parameter Update**: Update the weights and biases using the computed gradients.

## Usage

To run the project, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/Sudhan-Dahake/Optical-Character-Recognition.git
    ```

2. Install the required libraries:
    ```bash
    pip install numpy pandas matplotlib
    ```

3. Ensure you have the MNIST dataset file `MNIST_dataset.csv` in the project directory.

4. Run the main script:
    ```bash
    python Optical_Character_Recognition.py
    ```

## Results

The model achieves an accuracy of 88.8% on the MNIST dataset.
