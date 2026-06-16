# ML From Scratch

I am a first-year CS student working through machine learning by implementing
algorithms from scratch before touching any high-level libraries.

This repository is a learning journal, not a polished portfolio. Every notebook
prioritizes understanding over brevity — the goal is to be able to derive and
implement each algorithm from first principles, not to call sklearn in three lines.

---

## Projects

### Heart Disease Classifier
*Logistic regression from scratch on the UCI Heart Disease dataset*

Built without any ML libraries. Implements sigmoid, binary cross-entropy loss,
gradient descent, and evaluation metrics (accuracy, precision, recall, F1,
confusion matrix) entirely in NumPy.

The most useful thing I learned: without feature normalization, gradient descent
either diverges or converges so slowly it appears broken. Seeing this happen
visually made the math click in a way that reading about it didn't.

[View project →](projects/01-heart-disease-classifier)

---

## Course Progress

| Topic | Status | What I actually learned |
|-------|--------|------------------------|
| Simple Linear Regression | ✅ Done | How gradient descent works geometrically — the cost surface, not just the update rule |
| Multiple Linear Regression | ✅ Done | Why feature scaling is necessary, not just recommended — unscaled features make the cost surface extremely elongated and gradient descent zigzags |
| Logistic Regression | ✅ Done | How binary cross-entropy loss connects to maximum likelihood estimation |
| Overfitting and Regularization | ✅ Done | What lambda is actually doing — penalizing large weights, not penalizing complexity directly |
| Neural Networks — Forward Propagation | ✅ Done | How data flows through layers and why caching z and a during the forward pass is necessary for backpropagation |
| Neural Networks — TensorFlow Training | ✅ Done | Why logits + from_logits=True is numerically more stable than softmax in the output layer |
| Neural Networks — Multiclass & Softmax | ✅ Done | How sparse categorical cross-entropy handles multiclass problems and why the output layer stays linear |
| Neural Networks — Backpropagation | ✅ Done | That delta2 = a2 - y is an exact result, not an approximation — the chain rule cancels cleanly for sigmoid + binary cross-entropy |
| Advice for Applying ML | 🔲 Planned | Bias-variance tradeoff, error analysis, improving model performance |
| Decision Trees | 🔲 Planned | Decision trees, random forests, boosted trees |
| Unsupervised Learning | 🔲 Planned | Clustering and anomaly detection |
| Recommender Systems | 🔲 Planned | Collaborative filtering, content-based filtering |
| Reinforcement Learning | 🔲 Planned | State-action value functions |

---

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
│       ├── 01-neural-networks-forward-propagation/
│       ├── 02_tensorflow_training_workflow/
│       ├── 03_multiclass_softmax_activations/
│       └── 04-neural-networks-back-propagation/
│
├── projects/
│   └── 01-heart-disease-classifier/
│
├── README.md
├── requirements.txt
└── LICENSE
```

---

## How to Run

```bash
git clone https://github.com/MUHassanT/ML_From_Scratch.git
cd ML_From_Scratch
pip install -r requirements.txt
jupyter notebook
```

Open any folder and run cells top to bottom.

---

## Stack

Python · NumPy · Matplotlib · Pandas · Jupyter · TensorFlow (Course 2 onwards)

---

## Note

Most early notebooks use small synthetic datasets — the point is the algorithm,
not the data. Projects use real datasets to apply the same concepts to messier,
more realistic problems.

Code is written to be readable and correct, not fast. Optimization comes later.
