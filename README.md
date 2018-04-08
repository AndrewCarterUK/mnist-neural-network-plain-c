# MNIST Neural Network in C

This source code seeks to replicate the [MNIST For ML Beginners](https://www.tensorflow.org/versions/r1.1/get_started/mnist/beginners) tutorial from the Tensorflow website using plain C code.

The task is to recognise digits, such as the ones below, as accurately as possible.

![MNIST digits](https://www.tensorflow.org/versions/r1.1/images/MNIST.png)

## Contents

- [mnist.c](mnist.c): Glue code that runs the algorithm steps and reports algorithm accuracy
- [mnist_file.c](mnist_file.c): Retrieves images and labels from the MNIST dataset
- [neural_network.c](neural_network.c): Implements training and prediction routines for a simple neural network

## Usage

```sh
make
./mnist
```

## Description

The neural network implemented has one output layers and no hidden layers. Softmax activation is used, and this ensures that the output activations form a probability vector corresponding to each label. The cross entropy is used as a loss function.

The algorithm reaches an accuracy of around 92% over 1000 steps.

## Expected Output

```
Step 0000	Average Loss: 4.36	Accuracy: 0.152
Step 0001	Average Loss: 3.42	Accuracy: 0.188
Step 0002	Average Loss: 2.97	Accuracy: 0.298
Step 0003	Average Loss: 2.53	Accuracy: 0.319
Step 0004	Average Loss: 2.19	Accuracy: 0.412
Step 0005	Average Loss: 2.08	Accuracy: 0.437
Step 0006	Average Loss: 1.73	Accuracy: 0.468
Step 0007	Average Loss: 1.51	Accuracy: 0.447
Step 0008	Average Loss: 1.57	Accuracy: 0.496
Step 0009	Average Loss: 1.45	Accuracy: 0.516
Step 0010	Average Loss: 1.78	Accuracy: 0.559
...
```

![training evolution](https://res.cloudinary.com/andrewcarteruk/image/upload/v1523189356/training-evolution_hhbsfb.png)
