# ML From Scratch

This repository documents my journey of learning Machine Learning from scratch.

I am studying core machine learning concepts mainly through Andrew Ng's Machine Learning Specialization and implementing the main algorithms myself using Python, NumPy, and Matplotlib.

The goal is to understand how the algorithms work internally before using higher-level libraries such as scikit-learn.

## Repository Structure

```text
ML_From_Scratch/
│
├── course-1-supervised-machine-learning/
│   ├── 01-linear-regression-one-variable/
│   ├── 02-multiple-linear-regression/
│   ├── 03-logistic-regression-classification/
│   └── 04-overfitting-and-regularization/
│
├── course-2-advanced-learning-algorithms/
│   └── 01-neural-networks/
│
├── projects/
│   └── 01-heart-disease-classifier/
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

## Progress

| Course                                                                | Topic                                | Status      | Description                                                                                                                            |
| --------------------------------------------------------------------- | ------------------------------------ | ----------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| Course 1: Supervised Machine Learning                                 | Simple Linear Regression             | Completed   | Implemented linear regression with one variable using gradient descent                                                                 |
| Course 1: Supervised Machine Learning                                 | Multiple Linear Regression           | Completed   | Extended linear regression to multiple features, feature scaling, learning rate tuning, feature engineering, and polynomial regression |
| Course 1: Supervised Machine Learning                                 | Logistic Regression                  | Completed   | Implemented binary classification using logistic regression                                                                            |
| Course 1: Supervised Machine Learning                                 | Overfitting and Regularization       | Completed   | Explored polynomial features, overfitting, and regularized logistic regression                                                         |
| Course 2: Advanced Learning Algorithms                                | Neural Networks                      | In Progress | Learning basic neural network concepts and implementation                                                                              |
| Course 2: Advanced Learning Algorithms                                | Advice for Applying Machine Learning | Planned     | Model evaluation, bias and variance, error analysis, and improving model performance                                                   |
| Course 2: Advanced Learning Algorithms                                | Decision Trees                       | Planned     | Decision trees, random forests, and boosted trees                                                                                      |
| Course 3: Unsupervised Learning, Recommenders, Reinforcement Learning | Unsupervised Learning                | Planned     | Clustering and anomaly detection                                                                                                       |
| Course 3: Unsupervised Learning, Recommenders, Reinforcement Learning | Recommender Systems                  | Planned     | Collaborative filtering and content-based recommender systems                                                                          |
| Course 3: Unsupervised Learning, Recommenders, Reinforcement Learning | Reinforcement Learning               | Planned     | Basics of reinforcement learning and state-action value functions                                                                      |

## Topics Covered

### Course 1: Supervised Machine Learning

#### 01. Simple Linear Regression

Implemented simple linear regression from scratch using:

* Python
* NumPy
* Matplotlib
* Gradient descent

This includes:

* Defining the prediction function
* Calculating the cost function
* Computing gradients
* Updating parameters using gradient descent
* Visualizing the fitted regression line

#### 02. Multiple Linear Regression

Implemented multiple linear regression from scratch using:

* Multiple input features
* Vectorized prediction
* Cost function for multiple variables
* Gradient descent with multiple variables
* Feature scaling
* Learning rate comparison
* Feature engineering
* Polynomial regression

#### 03. Logistic Regression

Implemented logistic regression for binary classification using:

* Sigmoid function
* Logistic regression hypothesis
* Binary cross-entropy cost function
* Gradient descent
* Prediction threshold
* Classification accuracy
* Decision boundary visualization

#### 04. Overfitting and Regularization

Explored overfitting and regularization using logistic regression with nonlinear features.

This includes:

* Underfitting and overfitting
* Polynomial feature mapping
* Regularized cost function
* Regularized gradient descent
* Comparing different lambda values
* Understanding why training accuracy alone is not enough

### Course 2: Advanced Learning Algorithms

#### 01. Neural Networks

Currently learning neural network basics, including:

* Neurons and layers
* Forward propagation
* Activation functions
* Neural network architecture
* Basic implementation ideas

This section is currently in progress.

## Projects

### Heart Disease Classifier from Scratch

A binary classification project where I implemented logistic regression from scratch using NumPy on the UCI Heart Disease dataset.

The project includes data preprocessing, train/test splitting, feature normalization, gradient descent, and evaluation using accuracy, precision, recall, F1 score, and a confusion matrix.

[View project](projects/01-heart-disease-classifier)

## How to Run

Clone the repository:

```bash
git clone https://github.com/MUHassanT/ML_From_Scratch.git
cd ML_From_Scratch
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Open Jupyter Notebook:

```bash
jupyter notebook
```

Then open any topic or project folder and run the notebook cells from top to bottom.

## Tools Used

* Python
* NumPy
* Pandas
* Matplotlib
* Jupyter Notebook
* Git
* GitHub

## Learning Goals

Through this repository, I aim to:

* Understand machine learning algorithms from the ground up
* Implement algorithms manually before using high-level libraries
* Build clear intuition behind cost functions, gradients, and optimization
* Practice documenting technical projects clearly
* Build a strong foundation for more advanced ML and AI topics
* Compare manual implementations with library-based implementations later

## Next Topics

Planned topics include:

* Neural networks
* Model evaluation and error analysis
* Bias and variance
* Decision trees and ensemble methods
* Unsupervised learning
* Recommender systems
* Reinforcement learning
* scikit-learn implementations for comparison

## Note

This repository is part of my learning process. The code is written to prioritize understanding over optimization, so some implementations are intentionally simple and beginner-friendly.

Most datasets used in the early topic folders are small toy or synthetic datasets created for learning purposes. Projects are used to apply these concepts to more realistic datasets and machine learning workflows.
