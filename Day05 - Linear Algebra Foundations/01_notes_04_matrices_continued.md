# Day 5 — Matrices Continued

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Master Matrix Multiplication | Learn how to multiply matrices |
| 2 | Understand Matrix Dimensions | Learn when multiplication is possible |
| 3 | Connect to Neural Networks | See how matrix multiplication powers neural network layers |

---

## 1. Introduction

### Matrix Multiplication

**Matrix multiplication** is the core operation in neural networks. It combines information from rows and columns to transform data.

**Key Rule**: To multiply A × B:
- A must have n columns
- B must have n rows
- Result is (rows of A) × (columns of B)

### Why Matrix Multiplication Matters

Every forward pass in a neural network is matrix multiplication:
- Input × Weight Matrix = Output
- This happens at every layer
- GPUs are optimized specifically for this operation!

---

## 2. Deep-Dive Explanation

### How to Multiply

For A (m×n) × B (n×p) = C (m×p):

Element cᵢⱼ = sum of (aᵢₖ × bₖⱼ) for k = 1 to n

**Process**:
1. Take row i from A
2. Take column j from B
3. Multiply corresponding elements and sum

### Example

```
[1, 2]   [5, 6]   [1×5+2×7, 1×6+2×8]   [19, 22]
[3, 4] × [7, 8] = [3×5+4×7, 3×6+4×8] = [43, 50]
```

---

## 3. Instructor Examples

### Example 1: Basic Multiplication

**Question**: Multiply [1, 2; 3, 4] × [5; 6].

**Solution**:
- [1, 2; 3, 4] (2×2) × [5; 6] (2×1) = [1×5+2×6; 3×5+4×6] = [17; 39]
- Result is 2×1 vector

**AI Connection**: This is exactly what happens in a neural network: weight matrix × input vector = output vector.

---

### Example 2: Neural Network Layer

**Question**: Layer has 3 inputs, 2 neurons. W is 2×3, input x is 3×1. Calculate output.

**Solution**:
- Output = W × x
- 2×3 matrix × 3×1 vector = 2×1 vector
- Each element is a neuron's output

**AI Connection**: This is the forward pass computation at every layer.

---

### Example 3: Batch Processing

**Question**: Process 4 examples at once. Input matrix X is 4×3, weight W is 3×2.

**Solution**:
- Output = X × W
- 4×3 × 3×2 = 4×2 matrix
- Each row is one example's output

**AI Connection**: Processing batches is much more efficient than one example at a time.

---

## 4. Summary / Key Takeaways

- ✅ **Matrix multiplication**: (m×n) × (n×p) = (m×p)
- ✅ **Process**: Row of first × column of second, sum products
- ✅ **Neural networks**: Every layer is matrix multiplication
- ✅ **Batches**: Process multiple examples simultaneously
- ✅ Matrix multiplication is the computational heart of AI

