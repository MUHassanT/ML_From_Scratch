# Logistic Regression for Binary Classification

This notebook implements **logistic regression from scratch using NumPy**.

The goal is to understand how a binary classification model works internally before using machine learning libraries such as scikit-learn.

This project is part of my **machine learning from scratch** journey after completing Week 3 of Andrew Ng's Machine Learning course.

## Concepts Covered

* Binary classification
* Sigmoid function
* Logistic regression hypothesis
* Binary cross-entropy cost function
* Gradient descent
* Vectorized gradient calculation
* Prediction threshold
* Classification accuracy
* Decision boundary visualization

## What the Notebook Does

The notebook builds a simple logistic regression classifier using a small two-feature dataset.

The model learns to separate two classes using the equation:

```text
z = Xw + b
```

The sigmoid function converts this value into a probability:

```text
prediction = sigmoid(z)
```

A threshold of `0.5` is then used to convert the probability into a final class prediction:

```text
probability >= 0.5 → class 1
probability < 0.5  → class 0
```

## Implementation Details

The notebook includes from-scratch implementations of:

```python
sigmoid(z)
compute_cost(X, y, w, b)
compute_gradient(X, y, w, b)
gradient_descent(X, y, w, b, alpha, iterations)
predict(X, w, b)
```

The model is trained using gradient descent, and the cost is tracked over time to confirm that training is working.

## Result

The model achieves around **80% accuracy** on the toy dataset.

Since the dataset is small and manually created, the purpose of this notebook is not to build a production-level classifier. The main goal is to understand the core logic behind logistic regression.

## Visualizations

The notebook includes:

* A scatter plot of the binary classification dataset
* A sigmoid function plot
* A cost history plot
* A decision boundary plot

## Technologies Used

* Python
* NumPy
* Matplotlib
* Jupyter Notebook

## Key Learning

This notebook helped me understand that logistic regression is built by combining:

1. A linear model
2. The sigmoid function
3. Binary cross-entropy loss
4. Gradient descent
5. A classification threshold

Instead of treating logistic regression as a black-box algorithm, this notebook breaks down the main steps and implements them directly.
