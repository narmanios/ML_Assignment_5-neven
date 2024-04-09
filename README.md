# Multi-layer Perceptron Classifier

## Overview
This project demonstrates the use of a Multi-layer Perceptron (MLP) classifier for binary classification. The MLP is implemented using the `MLPClassifier` from the `sklearn.neural_network` module.

## Model Configuration
The MLP classifier is configured with the following parameters:
- `hidden_layer_sizes`: The number of neurons in each hidden layer. Several configurations were tried:
  - `(12, 36, 51, 73)`
  - `(25, 50, 75)`
  - `(50, 50)`
  - `(100, 50)`
- `max_iter`: The maximum number of iterations. The solver iterates until convergence or this number of iterations. In this example, it is set to 1000.

## Training the Model
The model is trained using the training data `data_train` and corresponding labels `y_train`. The performance of the model is evaluated on both the training and test sets.

## Performance Evaluation
The performance of the model is evaluated using a custom `BinaryClassificationPerformance` class, which computes various performance measures such as accuracy, precision, recall, F1 score, etc. The performance measures are printed for both the training and test sets.
