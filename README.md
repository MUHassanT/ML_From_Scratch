# ML From Scratch

This repository documents my journey of learning Machine Learning from scratch.

I am studying core machine learning concepts through Andrew Ng's Machine Learning courses and implementing the main algorithms myself using Python, NumPy, and Matplotlib.

The goal is to understand how the algorithms work internally before using higher-level libraries such as scikit-learn.

## Progress

| Topic                                | Status      | Description                                                                                                                            |
| ------------------------------------ | ----------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| Simple Linear Regression             | Completed   | Implemented linear regression with one variable using gradient descent                                                                 |
| Multiple Linear Regression           | Completed   | Extended linear regression to multiple features, feature scaling, learning rate tuning, feature engineering, and polynomial regression |
| Logistic Regression                  | Completed   | Implemented binary classification using logistic regression                                                                            |
| Overfitting and Regularization       | Completed   | Explored polynomial features, overfitting, and regularized logistic regression                                                         |
| Neural Networks                      | In Progress | Learning basic neural network concepts and implementation                                                                              |
| Advice for Applying Machine Learning | Planned     | Model evaluation, bias and variance, error analysis, and improving model performance                                                   |
| Decision Trees                       | Planned     | Decision trees, random forests, and boosted trees                                                                                      |
| Unsupervised Learning                | Planned     | Clustering and anomaly detection                                                                                                       |
| Recommender Systems                  | Planned     | Collaborative filtering and content-based recommender systems                                                                          |
| Reinforcement Learning               | Planned     | Basics of reinforcement learning and state-action value functions                                                                      |


## Topics Covered

### 01. Simple Linear Regression

Implemented simple linear regression from scratch using:

- Python
- NumPy
- Matplotlib
- Gradient descent

This includes:

- Defining the prediction function
- Calculating the cost function
- Computing gradients
- Updating parameters using gradient descent
- Visualizing the fitted regression line

### 02. Multiple Linear Regression

Implemented multiple linear regression from scratch using:

- Multiple input features
- Vectorized prediction
- Cost function for multiple variables
- Gradient descent with multiple variables
- Feature scaling
- Learning rate comparison
- Feature engineering
- Polynomial regression

### 03. Logistic Regression

Implemented logistic regression for binary classification using:

- Sigmoid function
- Logistic regression hypothesis
- Binary cross-entropy cost function
- Gradient descent
- Prediction threshold
- Classification accuracy
- Decision boundary visualization

### 04. Overfitting and Regularization

Explored overfitting and regularization using logistic regression with nonlinear features.

This includes:

- Underfitting and overfitting
- Polynomial feature mapping
- Regularized cost function
- Regularized gradient descent
- Comparing different lambda values
- Understanding why training accuracy alone is not enough

## Projects

### Heart Disease Classifier from Scratch

A binary classification project where I implemented logistic regression from scratch using NumPy on the UCI Heart Disease dataset.

The project includes data preprocessing, train/test splitting, feature normalization, gradient descent, and evaluation using accuracy, precision, recall, F1 score, and a confusion matrix.

[View project](projects/01-heart-disease-classifier)

## How to Run

1. Clone the repository.

    Command:

    git clone https://github.com/MUHassanT/ML_From_Scratch.git
    cd ML_From_Scratch

2. Install the required packages.

    Command:

    pip install -r requirements.txt

3. Open Jupyter Notebook.

    Command:

    jupyter notebook

4. Open any topic folder and run the notebook cells from top to bottom.

## Tools Used

- Python
- NumPy
- Matplotlib
- Jupyter Notebook
- Git
- GitHub

## Learning Goals

Through this repository, I aim to:

- Understand machine learning algorithms from the ground up
- Implement algorithms manually before using high-level libraries
- Build clear intuition behind cost functions, gradients, and optimization
- Document my learning process clearly
- Build a strong foundation for more advanced ML and AI topics
- Compare manual implementations with library-based implementations later

## Next Topics

Planned topics include:

- Neural networks
- Train, validation, and test splits
- Model evaluation metrics
- First end-to-end machine learning project
- scikit-learn implementations for comparison

## Note

This repository is part of my learning process. The code is written to prioritize understanding over optimization, so some implementations are intentionally simple and beginner-friendly.

Most datasets used here are small toy or synthetic datasets created for learning purposes. Future projects will include larger datasets, better evaluation workflows, and more realistic machine learning pipelines.
