# ML From Scratch

A structured collection of machine learning implementations, experiments, and projects built while studying supervised learning, neural networks, unsupervised learning, recommender systems, and reinforcement learning.

This repository is focused on understanding machine learning at the level of mathematics, implementation, and practical evaluation. The goal is not only to complete coursework, but to build the habit of turning concepts into working code and to develop a portfolio that is useful for research discussions, internship applications, and academic mentorship.

## Overview

`ML_From_Scratch` documents my progression through classical machine learning and introductory deep learning. The repository combines:

* algorithm implementations
* notebook-based experimentation
* mathematical intuition and derivations
* evaluation and model comparison
* a standalone applied project

The emphasis is on clarity, correctness, and independent understanding.

## Repository Structure

```text
ML_From_Scratch/
├── course-1-supervised-machine-learning/
│   ├── 01-linear-regression-one-variable/
│   ├── 02-multiple-linear-regression/
│   ├── 03-logistic-regression-classification/
│   └── 04-overfitting-and-regularization/
│
├── course-2-advanced-learning-algorithms/
│   ├── 01-neural-networks-forward-propagation/
│   ├── 02_tensorflow_training_workflow/
│   ├── 03_multiclass_softmax_activations/
│   ├── 04-neural-networks-back-propagation/
│   ├── 05-model-selection-and-evaluation/
│   ├── 06-bias_variance_learning_curves/
│   ├── 07_ml_development_process/
│   └── 08-decision-trees/
│
├── course-3-unsupervised-learning-recommenders-reinforcement-learning/
│   ├── 01-clustering/
│   ├── 02-anomaly-detection/
│   ├── 03-recommender-systems/
│   └── 04-reinforcement-learning/
│
├── projects/
│   └── heart-disease-classifier/
│
├── README.md
├── requirements.txt
└── LICENSE
```

## What This Repository Covers

### Supervised Learning

* Linear regression with one variable
* Multiple linear regression
* Logistic regression for classification
* Bias, variance, and regularization

### Advanced Learning Algorithms

* Neural network forward propagation
* Backpropagation
* Softmax and multiclass classification
* TensorFlow training workflow
* Model selection and evaluation
* Learning curves and error analysis
* Machine learning development process
* Decision trees

### Unsupervised Learning, Recommenders, and Reinforcement Learning

* Clustering
* Anomaly detection
* Recommender systems
* Reinforcement learning fundamentals

## Technical Stack

This repository uses:

* Python
* NumPy
* Pandas
* Matplotlib
* SciPy
* scikit-learn
* TensorFlow
* PyTorch
* Gymnasium
* ucimlrepo
* Jupyter
* ipykernel

The code and notebooks are organized to support both learning and experimentation.

## Learning Approach

Each topic is treated as more than a checklist item. The focus is on:

* understanding the underlying math
* implementing core ideas in code
* testing assumptions with experiments
* comparing model behavior
* documenting observations clearly

This approach is meant to build depth rather than shallow familiarity.

## Featured Project: [Heart Disease Classifier](project/heart-disease-classifier/)

The main standalone project in this repository is the **Heart Disease Classifier**, an applied machine learning project focused on binary classification for medical risk prediction. The core model implementation was built without scikit-learn.

### Project Highlights

* built on a real-world dataset from the UCI Machine Learning Repository
* implemented with Python and NumPy-first modeling choices
* includes data loading, preprocessing, training, and evaluation
* evaluates performance with more than just accuracy, with attention to precision, recall, and overall classification behavior

### Why This Project Matters

This project marks the transition from course exercises to an applied workflow. It demonstrates how a model can be developed, tested, and evaluated on a practical dataset while keeping the implementation understandable and easy to inspect.

## Skills Demonstrated

* translating mathematical ideas into code
* working with tabular data and numerical computation
* evaluating classification and regression models
* understanding optimization and learning dynamics
* debugging notebook-based workflows
* structuring technical work for review and portfolio use

## Current Status

This repository began with coursework, but its purpose is broader now. It is a growing implementation portfolio that reflects how I study machine learning: by rebuilding concepts, testing them, and extending them into projects.

## Future Direction

Planned future work may include:

* additional machine learning projects
* deeper experimentation with neural networks
* more applied work in AI and cybersecurity
* paper replication and research-style notebooks
* stronger model evaluation and interpretability work
* broader reinforcement learning experiments

## Acknowledgements

The structure and core topics in this repository were developed while completing the Machine Learning Specialization by DeepLearning.AI, taught by Andrew Ng. The implementations, organization, and project work in this repository are intended to go beyond passive course completion and reflect independent practice.

## License

This repository is licensed under the terms of the [LICENSE](LICENSE) file.

---
