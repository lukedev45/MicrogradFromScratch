# Micrograd From Scratch

This repository contains my *from-scratch* implementation and exploration of **Micrograd**, inspired by Andrej Karpathy’s YouTube lecture  
**“The spelled-out intro to neural networks and backpropagation: building micrograd.”**

The purpose of this project is to deeply understand how **automatic differentiation**, **backpropagation**, and **gradient-based learning** work internally — by implementing them manually in pure Python rather than relying on high-level frameworks.

---

## 📹 Lecture — Video Link

**Andrej Karpathy — The spelled-out intro to neural networks and backpropagation: building micrograd**

https://www.youtube.com/watch?v=VMj-3S1tku0

This lecture walks through:
- How neural networks learn from first principles
- How backpropagation works via the chain rule
- How to construct a tiny automatic differentiation engine
- How to use that engine to train a neural network

The explanation assumes only basic Python and introductory calculus, making it ideal for building strong foundations in deep learning.

---

## 🎯 Project Overview

Modern deep learning frameworks such as PyTorch or TensorFlow abstract away most of the machinery behind gradient computation and optimisation. While this is extremely powerful, it can hide *how* neural networks actually learn.

**Micrograd** strips everything down to the essentials.

This repository follows along with the Micrograd build to:
- Expose the mechanics of backpropagation
- Understand how computation graphs are constructed and traversed
- See exactly how gradients flow through a neural network
- Implement training using gradient descent from scratch

---

## 🔬 What Is Micrograd?

Micrograd is a **minimal automatic differentiation engine** that supports:
- Scalar-valued computation graphs
- Reverse-mode automatic differentiation (backpropagation)
- Gradient-based optimisation
- A small neural network API built on top of the autograd engine

Despite its simplicity, Micrograd demonstrates the same core ideas used in modern deep learning libraries.

---

## 🧠 Core Concepts Covered

This project focuses on understanding the following fundamental ideas:

### 🔹 Automatic Differentiation (Autograd)
Automatically computes derivatives of functions defined as code by tracking operations in a computation graph.

### 🔹 Backpropagation
Efficiently computes gradients by traversing the computation graph backward using the chain rule.

### 🔹 Computation Graphs
Directed graphs where:
- Nodes represent values
- Edges represent operations and dependencies  
These graphs allow gradients to be propagated correctly.

### 🔹 Gradient Descent
An optimisation algorithm that updates model parameters in the direction that minimises a loss function.

---

## 🧪 What This Repository Contains

This repository includes:
- A step-by-step construction of the `Value` class for gradient tracking
- Manual implementation of forward and backward passes
- Simple neural network components (neurons, layers, MLPs)
- Training loops using gradient descent
- Experiments inspired directly by the lecture

The focus is **clarity and learning**, not performance.

---

## 🚀 Learning Goals

By completing this project, the aim is to:
- Understand how neural networks work *under the hood*
- Gain intuition for gradients and optimisation
- Demystify PyTorch-style autograd systems
- Build confidence implementing ML systems from first principles

This knowledge directly transfers to larger-scale deep learning systems and research.

---

## 🛠️ Getting Started

Clone the repository:

```bash
git clone https://github.com/lukedev45/MicrogradFromScratch.git
cd MicrogradFromScratch
```
