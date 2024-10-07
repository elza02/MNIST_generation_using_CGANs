# CGAN for MNIST Generation

This project implements a Conditional Generative Adversarial Network (CGAN) for generating handwritten digits using the MNIST dataset. The goal is to create realistic images of digits conditioned on the class labels (0-9).

## Table of Contents
- [Introduction](#introduction)
- [Requirements](#requirements)
- [Dataset](#dataset)

## Introduction

Generative Adversarial Networks (GANs) are a class of machine learning frameworks where two neural networks, the generator and the discriminator, compete against each other. A CGAN extends GANs by conditioning both networks on additional information, allowing for more controlled image generation.

In this project, we leverage the MNIST dataset, which contains 70,000 images of handwritten digits (0-9), to train our CGAN to generate digits conditioned on specific labels.

## Requirements

- Python 3.x
- TensorFlow 2.x
- NumPy
- Matplotlib (for visualization)
- Other libraries (see `requirements.txt`)

## Dataset

The MNIST dataset can be downloaded using TensorFlow/Keras as follows:

```python
from tensorflow.keras.datasets import mnist
(x_train, y_train), (x_test, y_test) = mnist.load_data()
