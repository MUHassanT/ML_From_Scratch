# Overfitting and Regularization

This notebook explores overfitting and regularization using logistic regression.

It builds on the previous classification notebook by showing what happens when a model becomes more flexible through polynomial features, and how regularization can help control that flexibility.

## What This Notebook Covers

* Underfitting, good fit, and overfitting
* Polynomial feature mapping
* Logistic regression with nonlinear features
* Regularized cost function
* Regularized gradient descent
* The effect of different lambda values
* Training accuracy comparison

## Main Idea

A basic logistic regression model creates a linear decision boundary. However, some datasets cannot be separated well using a straight line.

To make the model more flexible, polynomial features are added. This allows logistic regression to learn more complex decision boundaries.

However, if the model becomes too flexible, it may overfit the training data. Overfitting means the model fits the training examples too closely instead of learning the general pattern.

Regularization helps reduce this problem by penalizing large weight values.

## Regularization

The regularized cost function adds an extra penalty term to the normal logistic regression cost:

```text
regularized cost = normal cost + regularization penalty
```

The regularization penalty is controlled by `lambda`.

* `lambda = 0`: no regularization
* Small `lambda`: weak regularization
* Large `lambda`: strong regularization

If `lambda` is too small, the model may overfit.

If `lambda` is too large, the model may underfit.

## Results

The model was trained using different values of `lambda`.

In the results, the model achieved the highest training accuracy when `lambda = 0`. This makes sense because without regularization, the model is more flexible and can fit the training data more closely.

However, higher training accuracy does not always mean the model is better overall. A model with perfect training accuracy may still perform poorly on unseen data if it has overfit.

To properly evaluate generalization, a separate validation or test set would be needed.

## Key Takeaways

* Polynomial features make logistic regression more powerful.
* More model flexibility can increase the risk of overfitting.
* Regularization reduces overfitting by discouraging large weights.
* The `lambda` parameter controls the strength of regularization.
* Regularization may reduce training accuracy, but it can improve generalization.
* Training accuracy alone is not enough to judge whether a model is good.

## Tools Used

* Python
* NumPy
* Matplotlib

## Status

Completed as part of my machine learning from scratch learning journey after studying classification and regularization in Andrew Ng's Machine Learning course.
