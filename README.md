# DPDLIGDO

## Introduction

This repository contains the codes that implement the experiments described in our paper "Differentially Private Deep Learning with Iterative Gradient
Descent Optimization" published at ACM Transactions on Data Science. In this paper, we propose a novel perturbed iterative gradient descent optimization
(PIGDO) algorithm and prove that this algorithm satisfies the differential privacy. A number of experiments demonstrate that our optimization algorithm can not only improve the model accuracy and training speed, but also achieve better privacy guarantees over the state-of-the-art algorithm while reaching the equivalent accuracy.
## Requirements

We uses TensorFlow to define deep learning models. Therefore, installing TensorFlow (>= 1.14) is a pre-requisite. For better performance, it is also recommended to install TensorFlow with GPU support (detailed instructions on how to do this are available in the TensorFlow installation documentation).

In addition to TensorFlow and its dependencies, other prerequisites are:

scipy >= 0.17

mpmath (for testing)

tensorflow_datasets

## Install Tensorflow Privacy

You can clone this old-version tensorflow privacy from GitHub repository into a directory of your choice:

https://github.com/chenlin0102/Differentially-private-GDO.git

You can then install the local package in "editable" mode in order to add it to your PYTHONPATH:

cd privacy
pip install -e .

## Quick Start
You can run our cifar10.py, mnist.py and fashion_mnist.py files to perform the experiments and change all the configurations (including dataset, dp_optimizer,  l2_norm_clip, noise_multiplier, num_microbatches, learning_rate and neural network architecture) to validate our experimental results. Finally, our codes are suitable for the colab and you can open the .ipynb files from https://github.com/chenlin0102/Differentially-private-GDO.git to run them on colab.
