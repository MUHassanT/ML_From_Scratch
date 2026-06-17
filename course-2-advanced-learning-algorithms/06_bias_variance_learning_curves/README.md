# Bias, Variance, and Learning Curves

This notebook explores practical techniques for diagnosing machine learning model performance through the lens of bias, variance, learning curves, and regularization.

Using a synthetic regression dataset, polynomial regression models of varying complexity are analyzed to investigate underfitting, overfitting, and generalization. The notebook focuses on understanding *why* a model performs the way it does and how practitioners can decide what to try next during the machine learning development process.

## Topics Covered

* Bias and Variance
* Underfitting and Overfitting
* Train/Cross-Validation/Test Splits
* Learning Curves
* Regularization
* Model Diagnostics
* Mean Squared Error (MSE)

## Experiments

### 1. Bias-Variance Diagnosis

Polynomial regression models of different degrees are trained and evaluated using training and cross-validation error.

This experiment demonstrates how model complexity influences performance and provides intuition for identifying high-bias and high-variance behavior.

### 2. Learning Curve Analysis

A high-complexity polynomial model is trained using progressively larger subsets of the training data.

Training and cross-validation errors are tracked as the dataset grows, allowing us to investigate how additional data affects generalization performance.

### 3. Regularization Experiment

Ridge Regression is applied with different regularization strengths to examine how penalizing model complexity influences training and validation performance.

This experiment illustrates that regularization must be validated empirically and is not always beneficial.

## Key Findings

* Model complexity alone does not determine performance.
* Learning curves provide valuable insight into bias and variance.
* Additional training data can improve generalization.
* Regularization introduces a trade-off between model flexibility and bias.
* Model improvement should be guided by evidence rather than assumptions.

## Tools Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-Learn

## Notebook

* `06_bias_variance_learning_curves.ipynb`
