# PAI_Pr2_BayesianNeuralNetworks
Project 2 for the course of Probabilistic Artificial Intelligence. Used Monte Carlo Dropout method to implement Bayesian Neural Networks for a task of image classification.
The training set consists of the original 20000 MNIST training images. The test set consists of a modified version of MNIST. The test images exhibit varying degrees of ambiguity and are further rotated by random angles. Ambiguity introduces aleatoric uncertainty since a true image label might not be uniquely identifiable. The rotations introduce epistemic uncertainty since the neural network only observes non-rotated images during training. Note that this is different from many typically studied settings in machine learning where the train and test data come from the same distribution.

# HOW TO EXECUTE
1. Download Docker
2. To run from Linux
  $ bash runner.sh

# SHORT REPORT
This task was solved using Monte Carlo Dropout method.
The neural network used, was implemented from scratch. It is a convolution neural network with many layers, but only 4 epochs (more epochs did not improve the performance as the optimum was reached very quickly).
To the neural network were added 2 dropout layers, with probability 0.25 and 0.5 respectively.

