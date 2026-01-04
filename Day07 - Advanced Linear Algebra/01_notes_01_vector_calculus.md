# Day 7 — Vector Calculus

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Gradients | Learn gradient as vector of partial derivatives |
| 2 | Apply to Functions | Calculate gradients of multivariable functions |
| 3 | Connect to AI | See how gradients guide optimization in high dimensions |

---

## 1. Introduction

### What is Vector Calculus?

**Vector calculus** extends calculus to functions of multiple variables. Key concept: **gradient**.

**Gradient** = vector pointing in direction of steepest increase, with magnitude = rate of increase.

### Why Vector Calculus Matters for AI

Gradients are the heart of neural network training:

- **Gradient Descent**: Uses gradient to minimize loss
- **Backpropagation**: Calculates gradients through network
- **Optimization**: Guides weight updates in high-dimensional spaces

---

## 2. Deep-Dive Explanation

### Gradient Definition

For function f(x, y), the gradient is:
**∇f = [∂f/∂x, ∂f/∂y]**

Vector of partial derivatives.

### Properties

- **Direction**: Points toward steepest increase
- **Magnitude**: Rate of increase in that direction
- **Minimization**: Move opposite to gradient (gradient descent)

---

## 3. Instructor Examples

### Example 1: Simple Gradient

**Question**: Find gradient of f(x, y) = x² + y².

**Solution**:
- ∂f/∂x = 2x
- ∂f/∂y = 2y
- ∇f = [2x, 2y]

**AI Connection**: Loss functions in neural networks are multivariable. Gradients tell us how to update each weight.

---

### Example 2: Gradient Descent

**Question**: At point (1, 1) for f(x, y) = x² + y², what's the gradient? Which direction should we move to minimize?

**Solution**:
- ∇f(1, 1) = [2, 2]
- To minimize, move opposite: direction = -[2, 2] = [-2, -2]
- This points toward (0, 0), the minimum!

**AI Connection**: This is exactly gradient descent: w_new = w_old - α·∇L (move opposite to gradient).

---

## 4. Summary / Key Takeaways

- ✅ **Gradient**: Vector of partial derivatives ∇f = [∂f/∂x, ∂f/∂y, ...]
- ✅ **Direction**: Points toward steepest increase
- ✅ **Gradient Descent**: Move opposite to gradient to minimize
- ✅ **AI Connection**: Core of neural network training and optimization
- ✅ Vector calculus enables optimization in high-dimensional weight spaces

