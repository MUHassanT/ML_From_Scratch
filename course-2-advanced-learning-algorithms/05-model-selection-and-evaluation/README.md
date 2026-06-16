# Model Evaluation and Selection

This notebook explores how machine learning models should be evaluated and selected using training, cross-validation, and test datasets.

Using a synthetic regression dataset, polynomial regression models of varying complexity are trained and compared. The notebook demonstrates how validation performance can be used to guide model selection and highlights the relationship between model complexity and generalization.

## Topics Covered

* Train, Cross-Validation, and Test Sets
* Model Evaluation
* Model Selection
* Generalization
* Underfitting and Overfitting
* Cross-Validation
* Mean Squared Error (MSE)

## Experiment Overview

A noisy sinusoidal dataset is generated and split into training, cross-validation, and test sets.

Polynomial regression models with different degrees are trained and evaluated. Their performance is compared using Mean Squared Error across all three datasets to investigate how increasing model complexity affects generalization.

## Key Findings

* Low-complexity models may underfit the underlying pattern.
* Increasing model complexity can significantly improve performance.
* Excessive complexity may lead to overfitting.
* Cross-validation provides a reliable mechanism for model selection.
* Training performance alone is insufficient for choosing the best model.

## Tools Used

* Python
* NumPy
* Matplotlib
* Scikit-Learn

## Notebook

* `05-model-selection-and-evaluation.ipynb`
