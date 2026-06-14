# Backpropagation From Scratch

A from-scratch implementation of backpropagation using NumPy, with no 
reliance on TensorFlow or any automatic differentiation library.

## What This Is

The previous notebook in this series used TensorFlow to train a neural 
network. TensorFlow handles backpropagation automatically, which means 
you can train a model without understanding what is happening during the 
backward pass.

This notebook removes that abstraction entirely. Every gradient is computed 
manually using the chain rule, and a numerical gradient check confirms that 
the implementation is correct.

## What I Implemented

- Sigmoid activation and its derivative
- Forward propagation through a two-layer network
- Binary cross-entropy loss
- Backpropagation — computing gradients layer by layer
- Gradient descent parameter updates
- Numerical gradient checking to verify correctness

## Key Result

The network achieved 99.5% training accuracy on a binary classification 
dataset. The gradient check confirmed that all analytical gradients matched 
numerical approximations to within 1e-7, well below the 1e-5 threshold.

## What I Learned

Before implementing this, I understood backpropagation as "the model goes 
backwards and fixes the weights." That description is not wrong but skips 
everything that actually matters.

The backward pass is the chain rule applied repeatedly. At each layer you 
compute delta — how much the loss changes with respect to the pre-activation 
z — and use it to get the weight gradients. The pattern is identical at every 
layer.

The most surprising result was that the output layer gradient simplifies to 
delta2 = a2 - y. The sigmoid derivative and the cross-entropy derivative 
cancel cleanly, leaving just the prediction error.

## Network Architecture

Input (2) → Dense (3, sigmoid) → Dense (1, sigmoid) → Output

## Tools Used

- Python
- NumPy
- Matplotlib

## Next Step

Extend backpropagation to a deeper network and observe how gradients shrink 
in earlier layers — the vanishing gradient problem that motivated ReLU and 
modern activation functions.