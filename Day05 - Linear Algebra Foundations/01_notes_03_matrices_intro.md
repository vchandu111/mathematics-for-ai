# Day 5 — Matrices Intro

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Matrices | Learn what matrices are and their structure |
| 2 | Matrix Operations | Master matrix addition, scalar multiplication |
| 3 | Connect to AI | See how matrices represent weights and transformations in neural networks |

---

## 1. Introduction

### What is a Matrix?

A **matrix** is a rectangular array of numbers arranged in rows and columns. It's like a table of numbers.

**Notation**: 
```
A = [a₁₁  a₁₂]
    [a₂₁  a₂₂]
```

- Rows go horizontally
- Columns go vertically
- aᵢⱼ = element in row i, column j

### Why Matrices Matter for AI

Matrices are everywhere in AI:

- **Neural Network Weights**: Each layer's weights are a matrix
- **Data**: Batches of data points form matrices
- **Transformations**: Matrices transform input to output
- **Efficiency**: Matrix operations are highly optimized (GPUs excel at this)

### Real-World Analogy

Think of a matrix like a spreadsheet:
- **Rows** = different data points or examples
- **Columns** = different features or dimensions
- **Matrix multiplication** = combining information across rows and columns

In AI: Input matrix (batch of images) × Weight matrix = Output matrix (predictions)

---

## 2. Deep-Dive Explanation

### Matrix Dimensions

A matrix with m rows and n columns is called an **m×n matrix**.

**Examples**:
- [1, 2; 3, 4] is a 2×2 matrix (2 rows, 2 columns)
- [1, 2, 3; 4, 5, 6] is a 2×3 matrix (2 rows, 3 columns)

### Matrix Addition

Add corresponding elements:
```
[a, b]   [e, f]   [a+e, b+f]
[c, d] + [g, h] = [c+g, d+h]
```

**Rule**: Matrices must have the same dimensions.

### Scalar Multiplication

Multiply every element by the scalar:
```
k × [a, b]   [ka, kb]
    [c, d] = [kc, kd]
```

---

## 3. Instructor Examples

### Example 1: Matrix Structure

**Question**: What are the dimensions of matrix A = [1, 2, 3; 4, 5, 6]?

**Solution**:
- 2 rows, 3 columns
- This is a 2×3 matrix
- Element a₁₂ = 2 (row 1, column 2)

**AI Connection**: In neural networks, a weight matrix might be 784×128 (784 inputs, 128 neurons), where each row represents connections to one neuron.

---

### Example 2: Matrix Addition

**Question**: Add [1, 2; 3, 4] + [5, 6; 7, 8].

**Solution**:
- [1+5, 2+6; 3+7, 4+8] = [6, 8; 10, 12]

**AI Connection**: In neural networks, we might add bias matrices or combine multiple weight updates.

---

### Example 3: Scalar Multiplication

**Question**: Calculate 3 × [2, 4; 1, 3].

**Solution**:
- 3 × [2, 4; 1, 3] = [6, 12; 3, 9]

**AI Connection**: Learning rate multiplies gradient matrices during weight updates: w_new = w_old - α·∇L (scalar times matrix).

---

### Example 4: Weight Matrix in AI

**Question**: A neural network layer has 3 inputs and 2 neurons. What are the dimensions of the weight matrix?

**Solution**:
- 2 rows (one per neuron) × 3 columns (one per input)
- This is a 2×3 matrix
- Each row represents weights for one neuron

**AI Connection**: This is exactly how neural network layers are structured. The weight matrix W transforms input vector x to output: y = W·x.

---

## 4. Summary / Key Takeaways

- ✅ **Matrix** = rectangular array of numbers (rows × columns)
- ✅ **Matrix Addition**: Add corresponding elements (same dimensions required)
- ✅ **Scalar Multiplication**: Multiply every element by the scalar
- ✅ **AI Connection**: Weight matrices in neural networks; data organized as matrices
- ✅ Matrix dimensions matter: m×n matrix has m rows and n columns

