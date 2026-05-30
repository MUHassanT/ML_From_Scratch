# Week 2: Multiple Linear Regression

This folder contains my implementation of multiple linear regression from scratch.

The goal of this week was to understand how linear regression extends from one input feature to multiple input features, and how techniques like feature scaling, learning rate selection, and polynomial regression affect model training.

## Topics Covered

* Multiple linear regression
* Vectorized prediction
* Cost function for multiple variables
* Gradient descent with multiple variables
* Feature scaling
* Learning rate comparison
* Polynomial regression

## What I Implemented

In this notebook, I implemented the main parts of multiple linear regression manually using Python and NumPy.

This includes:

* creating a dataset with multiple input features
* defining the prediction function
* calculating the cost function
* computing gradients for multiple weights and the bias
* updating parameters using gradient descent
* training the model without feature scaling
* applying z-score normalization
* training the model after feature scaling
* comparing different learning rates
* creating polynomial features
* training a polynomial regression model
* visualizing the polynomial regression fit

## Model

The multiple linear regression model is:

```text
f(x) = w · x + b
```

Where:

* `x` is a vector of input features
* `w` is a vector of weights
* `b` is the bias term
* `f(x)` is the predicted output

Unlike simple linear regression, where there is only one input feature, multiple linear regression allows the model to learn from several features at once.

## Feature Scaling

Feature scaling was used to improve gradient descent.

I used z-score normalization:

```text
x_scaled = (x - mean) / standard_deviation
```

This helped bring all features into a similar range and made training more stable.

## Learning Rate Comparison

I also tested different learning rates to observe how they affect gradient descent.

A small learning rate can make training slow, while a large learning rate can cause the cost to increase or become unstable.

The goal was to choose a learning rate that allowed the cost to decrease smoothly over time.

## Polynomial Regression

Polynomial regression was implemented by creating new features from an existing feature.

For example:

```text
x, x², x³
```

This allowed the linear regression model to fit curved patterns while still using the same gradient descent algorithm.

## Tools Used

* Python
* NumPy
* Matplotlib
* Jupyter Notebook

## Key Takeaway

This week helped me understand how linear regression can be extended beyond one variable.

I learned that multiple linear regression uses the same basic ideas as simple linear regression, but with more features and weights.

I also learned that feature scaling and learning rate selection are important for efficient gradient descent, and that polynomial regression is a way to model non-linear patterns using linear regression.
