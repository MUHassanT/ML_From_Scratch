# Tree-Based Machine Learning: From Decision Trees to XGBoost

A comprehensive, mathematics-first exploration of tree-based machine learning algorithms, progressing from information theory and decision trees to modern ensemble methods such as Random Forests, Gradient Boosting, and XGBoost.

## Overview

Tree-based models are among the most widely used machine learning algorithms due to their ability to model nonlinear relationships, capture complex feature interactions, and deliver strong predictive performance with minimal preprocessing.

This notebook develops the theory and intuition behind tree-based learning from first principles. Beginning with Shannon's information theory, we derive entropy and information gain, examine how decision trees select optimal splits, and then explore how ensemble techniques overcome the limitations of individual trees.

The notebook concludes with an introduction to XGBoost, one of the most successful machine learning algorithms in both industry and competitive data science.

---

## Topics Covered

### 1. Decision Trees and Recursive Partitioning

* Hierarchical decision making
* Recursive partitioning of feature space
* Axis-aligned splits
* Decision boundaries

### 2. Information Theory Foundations

* Self-information
* Entropy
* Uncertainty quantification
* Entropy visualization and interpretation

### 3. Information Gain

* Weighted child entropy
* Information gain derivation
* Split evaluation
* Manual worked examples

### 4. Split Selection

* Candidate threshold generation
* Exhaustive threshold search
* Best split identification
* Computational considerations

### 5. Building Decision Trees

* Recursive tree construction
* Stopping criteria
* Tree visualization
* Model interpretation

### 6. Overfitting and Generalization

* Bias-variance tradeoff
* Effect of tree depth
* Training vs testing performance
* Model complexity analysis

### 7. Random Forests

* Bootstrap sampling
* Out-of-Bag (OOB) estimation
* Random feature selection
* Variance reduction through bagging

### 8. Gradient Boosting

* Sequential learning
* Residual fitting
* Functional gradient descent
* Learning rate intuition

### 9. XGBoost

* Regularized objective function
* First- and second-order optimization
* Split gain formula
* Regularization techniques
* Practical implementation

---

## Mathematical Concepts

The notebook derives and discusses:

### Entropy

$$
H(S) = -\sum_i p_i \log_2(p_i)
$$

### Information Gain

$$
IG = H(\text{Parent}) - H(\text{Children})
$$

### Bootstrap Sampling

$$
\left(1-\frac{1}{n}\right)^n
\rightarrow
e^{-1}
$$

### Gradient Boosting Update Rule

$$
F_m(x) = F_{m-1}(x) + \eta h_m(x)
$$

### XGBoost Objective Function

$$
\text{Obj} = L + \Omega(f)
$$

### XGBoost Split Gain

$$
\text{Gain} = \frac{1}{2}\left(\frac{G_L^2}{H_L+\lambda} + \frac{G_R^2}{H_R+\lambda} - \frac{G^2}{H+\lambda}\right) - \gamma
$$

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-Learn
* XGBoost

---

## Learning Outcomes

After completing this notebook, readers should be able to:

* Explain how decision trees construct decision boundaries
* Compute entropy and information gain
* Understand tree split selection
* Analyze overfitting in tree-based models
* Explain the intuition behind bagging and boosting
* Understand how Random Forests reduce variance
* Understand how Gradient Boosting reduces bias
* Explain the key innovations introduced by XGBoost

---

## References

1. Claude E. Shannon — *A Mathematical Theory of Communication* (1948)
2. Leo Breiman — *Random Forests* (2001)
3. Jerome Friedman — *Greedy Function Approximation: A Gradient Boosting Machine* (2001)
4. Tianqi Chen & Carlos Guestrin — *XGBoost: A Scalable Tree Boosting System* (2016)
5. Hastie, Tibshirani & Friedman — *The Elements of Statistical Learning*
6. Aurélien Géron — *Hands-On Machine Learning with Scikit-Learn, Keras & TensorFlow*
