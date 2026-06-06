# Simple Linear Regression

This folder contains my implementation of simple linear regression from scratch.

The goal of this week was to understand how a basic machine learning model learns a relationship between one input feature and one output value using gradient descent.

## Topics Covered

* Simple linear regression
* Model prediction
* Cost function
* Gradient descent
* Parameter updates
* Data visualization
* Regression line fitting

## What I Implemented

In this notebook, I implemented the main parts of linear regression manually using Python and NumPy.

This includes:

* defining the prediction function
* calculating the cost using mean squared error
* computing gradients for `w` and `b`
* updating parameters using gradient descent
* training the model over multiple iterations
* visualizing the final fitted line using Matplotlib

## Model

The simple linear regression model used is:

```text
f(x) = wx + b
```

Where:

* `x` is the input feature
* `w` is the weight/slope
* `b` is the bias/intercept
* `f(x)` is the predicted output

## Cost Function

The cost function measures how far the model's predictions are from the actual values.

The goal of training is to minimize this cost.

```text
J(w, b) = (1 / 2m) * sum((f(x) - y)^2)
```

## Gradient Descent

Gradient descent was used to update the parameters `w` and `b`.

The model repeatedly:

1. makes predictions
2. calculates the error
3. computes gradients
4. updates the parameters
5. reduces the cost over time

## Tools Used

* Python
* NumPy
* Matplotlib
* Jupyter Notebook

## Key Takeaway

This week helped me understand how a machine learning model can learn from data by gradually adjusting its parameters.

Instead of using a built-in machine learning library, I implemented the algorithm from scratch to understand what happens internally during training.
