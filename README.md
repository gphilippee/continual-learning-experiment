# Experiments on Continual Learning (CL)

Authors: Mathys Noir, Thomas Bersani, Guillaume Philippe

A repository of experiments with basic datasets (MNIST, FashionMNIST and permuted MNIST) and neural networks (fully-connected).

## Architecture

All experiments are made with a fully-connected networks with 2 hidden layers. They have 4096 neurons each. The output layer has 10 neurons (one for each class).

## Notebooks

## catastrophic_forgetting.ipynb

Observe catastrophic forgetting with training on MNIST first and Fashion-MNIST next.

## rehearsal_approach.ipynb

Try a rehearsal approach. We train sequentially on MNIST and Fashion-MNIST. At the end of each epoch, we train on a batch of 4096 samples from MNIST.

## dynamic_architecture.ipynb

Here, we decompose the output layer in two. 10 neurons for MNIST and 10 neurons for Fashion-MNIST.
At the end of a batch, we backpropagate only on the neurons that correspond to the current task.

## synaptic_metaplasticity.ipynb

We implement the method from the paper: Laborieux et al. Synaptic metaplasticity in binarized neural networks.