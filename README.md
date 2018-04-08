# MNIST Neural Network in C

This source code seeks to replicate the [MNIST For ML Beginners](https://www.tensorflow.org/versions/r1.1/get_started/mnist/beginners) tutorial from the Tensorflow website using straight forward C code.

## Contents

- `mnist.c`: Glue code that runs the algorithm steps and reports algorithm accuracy
- `mnist_file.c`: Retrieves images and labels from the MNIST dataset
- `neural_network.c`: Implements training and prediction routines for a simple neural network

## Usage

```sh
make
./mnist
```

## Description

The neural network implemented has one output layers and no hidden layers. Softmax activation is used, and this ensures that the output activations form a probability vector corresponding to each label. The cross entropy is used as a loss function.

The algorithm reaches an accuracy of around 92%.
