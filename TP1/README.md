# Backpropagation Derivation for MLP

We will derive backpropagation for a Multi-Layer Perceptron (MLP) with **one hidden layer**, trained using **Softmax** + **Cross-Entropy loss**.

## 1. Problem Setup

A **Multi-Layer Perceptron (MLP)** with one hidden layer consists of:

- **Input layer**: $X$ (size: $m \times  n_x$)
- **Hidden layer**: with tanh activation
- **Output layer**: with softmax activation

The parameters of the network:

- $W_1$ (weights between input and hidden layer, size $n_h \times (n_x+1) $ )
- $W_2$ (weights between hidden and output layer, size $n_y \times (n_h+1) $ )

## 2. Forward Propagation

### Step 1: Compute Hidden Layer Activation

We compute the linear transformation:

$$ Z_1 = W_1\: A_0 $$

where:

- $A_0 =[1; X^T]$

### Step 2: Compute Output Layer Activation
