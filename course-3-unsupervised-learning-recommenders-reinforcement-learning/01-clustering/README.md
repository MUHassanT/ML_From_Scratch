# K-Means Clustering From Scratch

This project implements the K-Means clustering algorithm from scratch using NumPy and explores its behavior on a synthetic dataset.

The notebook covers the mathematical intuition behind clustering, the implementation of core K-Means components, the effect of different values of K, and the Elbow Method for cluster selection.

---

## Overview

K-Means is an unsupervised learning algorithm that partitions data into K clusters by minimizing the distance between data points and their assigned cluster centroids.

The algorithm iteratively performs:

1. Assignment Step
   - Assign each data point to the nearest centroid.

2. Update Step
   - Recompute centroid positions as the mean of assigned points.

These steps repeat until convergence.

---

## Features

- K-Means implementation from scratch using NumPy
- Synthetic dataset generation using `make_blobs`
- Closest centroid assignment
- Centroid recomputation
- Full K-Means training loop
- Cluster visualization
- Comparison of different K values
- Elbow Method for selecting K
- Discussion of computational complexity, advantages, and limitations

---

## Mathematical Objective

K-Means minimizes the following objective function:

$$
J(c^{(1)},...,c^{(m)},\mu_1,...,\mu_K)
=
\frac{1}{m}
\sum_{i=1}^{m}
\left\|x^{(i)}-\mu_{c^{(i)}}\right\|^2
$$

where:

- $x^{(i)}$ is a training example
- $c^{(i)}$ is the assigned cluster
- $\mu_k$ is the centroid of cluster $k$

---

## Project Structure

```text
05_KMeans_Clustering/
│
├── KMeans_From_Scratch.ipynb
└── README.md
```

---

## Key Components

### Finding Closest Centroids

Assigns each example to the nearest centroid using Euclidean distance.

### Computing Centroids

Updates centroid locations by computing the mean of all points assigned to each cluster.

### Running K-Means

Alternates between assignment and update steps until convergence.

### Cost Function

Measures clustering quality using the average squared distance between points and their assigned centroids.

### Elbow Method

Evaluates clustering cost across multiple K values to identify an appropriate number of clusters.

---

## Results

The notebook demonstrates:

- Successful clustering of synthetic data
- The impact of different K values
- How clustering cost decreases as K increases
- How the Elbow Method can help select a suitable number of clusters

For the generated dataset, the elbow typically occurs around **K = 3**, which aligns with the true underlying cluster structure.

---

## Computational Complexity

Let:

- m = number of examples
- n = number of features
- K = number of clusters
- T = number of iterations

The overall complexity of K-Means is:

$$
O(TmKn)
$$

This makes K-Means computationally efficient and suitable for large datasets.

---

## Limitations

- Requires specifying K beforehand
- Sensitive to centroid initialization
- Sensitive to outliers
- Assumes approximately spherical clusters
- May converge to a local optimum

---

## Technologies Used

- Python
- NumPy
- Matplotlib
- Scikit-Learn (dataset generation only)

---

## Learning Outcomes

Through this project, I gained hands-on experience with:

- Unsupervised learning
- Cluster-based data exploration
- Iterative optimization algorithms
- Distance-based learning methods
- Model selection using the Elbow Method

---

## References

- Machine Learning Specialization — Andrew Ng
- K-Means Clustering Algorithm
- Scikit-Learn Documentation