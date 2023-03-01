# Experiments on Continual Learning (CL)

A repository of experiments with basic datasets and convolution networks

## cnn.ipynb

Observe catastrophic forgetting with MNIST and Fashion-MNIST tasks.

## rehearsal_cnn.ipynb

Try a rehearsal approach. We train sequentially on MNIST and Fashion-MNIST. At the end of each epoch, we train on a batch of MNIST. At the end, we observe better results.
