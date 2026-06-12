# TensorFlow Training Workflow

This notebook covers the basic workflow for training a neural network using TensorFlow/Keras.

The goal of this notebook is to understand how a neural network is built, compiled, trained, evaluated, and used for predictions using the high-level TensorFlow API.

## Notebook

`02_tensorflow_training_workflow.ipynb`

## Topics Covered

* Creating a simple binary classification dataset
* Visualizing the dataset
* Splitting data into training and test sets
* Normalizing input features
* Building a neural network using the Keras `Sequential` API
* Adding `Dense` layers
* Using ReLU activation in hidden layers
* Using sigmoid activation for binary classification
* Compiling a model with a loss function and optimizer
* Training the model using `model.fit()`
* Tracking training loss and accuracy
* Evaluating the model on test data
* Making predictions using `model.predict()`
* Converting predicted probabilities into class labels
* Checking accuracy manually with NumPy

## Model Architecture

The model used in this notebook is a small neural network for binary classification.

```python
model = Sequential(
    [
        tf.keras.Input(shape=(2,)),
        Dense(8, activation="relu"),
        Dense(4, activation="relu"),
        Dense(1, activation="sigmoid")
    ],
    name="binary_classification_model"
)
```

The final layer uses sigmoid activation because the task is binary classification.

## Training Workflow

The TensorFlow training process follows this general pipeline:

```text
build model → compile model → train model → evaluate model → make predictions
```

During training, TensorFlow handles the internal training loop automatically. This includes:

* forward propagation
* loss calculation
* backpropagation
* parameter updates

## Key Learning

This notebook helped me understand how TensorFlow simplifies neural network training through the Keras API.

Instead of manually writing the full training loop, TensorFlow allows the model to be trained using:

```python
model.compile()
model.fit()
model.evaluate()
model.predict()
```

The main takeaway is that TensorFlow automates the training process, but the underlying ideas are still the same: predictions are made, loss is calculated, gradients are computed, and parameters are updated.

## Tools Used

* Python
* NumPy
* Matplotlib
* TensorFlow
* Keras

## Next Steps

Backpropagation will be explored separately from scratch in a later notebook to better understand what TensorFlow does internally during training.