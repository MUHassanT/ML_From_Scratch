# Multiclass Classification, Softmax, and Activation Functions

This folder contains a notebook on multiclass classification using TensorFlow/Keras.

The goal of this notebook is to understand how neural networks handle problems with more than two classes, especially through logits, softmax, and sparse categorical cross-entropy.

## Notebook

`03_multiclass_softmax_activations.ipynb`

## Topics Covered

* Binary vs multiclass classification
* Creating a simple three-class dataset
* Visualizing multiclass data
* Train/test splitting
* Feature normalization
* Implementing softmax manually with NumPy
* Understanding logits
* Building a multiclass neural network with TensorFlow/Keras
* Using ReLU activation in hidden layers
* Using a linear output layer for logits
* Training with `SparseCategoricalCrossentropy(from_logits=True)`
* Converting logits into probabilities using softmax
* Converting probabilities into predicted class labels
* Plotting training loss and accuracy
* Evaluating test performance
* Comparing sigmoid, ReLU, and linear activations
* Choosing output layer activations based on the problem type

## Model Architecture

The model uses a small feedforward neural network:

```python
model = Sequential(
    [
        tf.keras.Input(shape=(2,)),
        Dense(16, activation="relu"),
        Dense(8, activation="relu"),
        Dense(3, activation="linear")
    ],
    name="multiclass_classification_model"
)
```

The final layer has 3 output units because the dataset has 3 classes.

## Why Linear Output Instead of Softmax?

For multiclass classification, the model can either:

1. output probabilities using a softmax activation, or
2. output raw logits and let the loss function handle softmax internally.

This notebook uses the second approach:

```python
SparseCategoricalCrossentropy(from_logits=True)
```

This is usually preferred because TensorFlow can compute the softmax and cross-entropy together in a more numerically stable way.

## Key Learning

The main idea is that multiclass classification requires the model to output one score per class.

```text
logits → softmax → class probabilities → predicted class
```

The predicted class is the class with the highest probability.

## Tools Used

* Python
* NumPy
* Matplotlib
* TensorFlow
* Keras

## Next Step

The next notebook will focus on backpropagation from scratch to understand what TensorFlow does internally during training.
