# Handwritten Digit Recognition using TensorFlow & Keras

A beginner Deep Learning project that classifies handwritten digits (0–9) using the MNIST dataset. The project explores Neural Networks, hyperparameter tuning, overfitting analysis, and regularization techniques using TensorFlow and Keras.

## Project Overview

The goal of this project is to build a neural network capable of recognizing handwritten digits from grayscale images.

The project goes beyond basic model training by experimenting with:

- Different numbers of neurons
- Additional hidden layers
- Different epoch counts
- Dropout regularization
- Training and validation performance analysis

## Dataset

MNIST Dataset

- 70,000 handwritten digit images
- 28×28 grayscale images
- 10 classes (digits 0–9)

Dataset Split:

- Training Samples: 60,000
- Testing Samples: 10,000

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Jupyter Notebook

## Neural Network Architecture

Input Layer (28×28)

↓

Flatten Layer

↓

Dense(256, ReLU)

↓

Dropout(0.2)

↓

Dense(128, ReLU)

↓

Dense(10, Softmax)

## Results

| Model Configuration | Test Accuracy |
|--------------------|---------------|
| Dense(128), 5 Epochs | 97.78% |
| Dense(256), 10 Epochs | 97.68% |
| Dense(256) + Dense(128) | 97.85% |
| With Dropout(0.2) | Improved Generalization |

## Experiments Performed

### Experiment 1: Increasing Neurons

Changed hidden layer size from 128 to 256 neurons.

Observation:
Increasing neurons alone did not improve performance significantly.

### Experiment 2: Adding an Extra Hidden Layer

Added an additional Dense(128) layer.

Observation:
A deeper network slightly improved accuracy.

### Experiment 3: Overfitting Analysis

Trained the model for additional epochs and monitored training and validation metrics.

Observation:
Validation loss increased while training loss decreased, indicating overfitting.

### Experiment 4: Dropout Regularization

Added Dropout(0.2) between hidden layers.

Observation:
Overfitting was reduced and model generalization improved.

## Key Learnings

- Built a Neural Network using TensorFlow and Keras
- Learned image classification fundamentals
- Understood activation functions and softmax output
- Performed hyperparameter tuning
- Learned to identify overfitting
- Applied Dropout regularization
- Visualized training and validation metrics

## Future Improvements

- Implement Convolutional Neural Networks (CNNs)
- Add Early Stopping
- Build a Streamlit web application
- Deploy the model online

## Author

Chinmay Mohite

Computer Science Engineering Student | Data Science & Machine Learning Enthusiast