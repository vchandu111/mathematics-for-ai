# Day 7 — Eigenvectors & Eigenvalues Continued

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Eigendecomposition | Learn how matrices decompose using eigenvectors |
| 2 | Apply to Data Analysis | See how eigendecomposition reveals structure |
| 3 | Connect to Advanced AI | Understand SVD, spectral methods, and advanced techniques |

---

## 1. Introduction

### Eigendecomposition

A matrix A can be decomposed as:
**A = Q·Λ·Q⁻¹**

Where:
- Q = matrix of eigenvectors
- Λ = diagonal matrix of eigenvalues

This reveals the structure of the transformation.

### Why Eigendecomposition Matters

- **PCA**: Eigendecomposition of covariance matrix
- **SVD**: Related to eigendecomposition
- **Matrix Powers**: Aⁿ = Q·Λⁿ·Q⁻¹ (efficient computation)
- **Understanding Transformations**: Reveals how matrix acts on space

---

## 2. Deep-Dive Explanation

### Eigendecomposition Formula

For diagonalizable matrix A:
- A = Q·Λ·Q⁻¹
- Columns of Q are eigenvectors
- Λ has eigenvalues on diagonal

### Properties

- **Symmetric matrices**: Always diagonalizable, Q is orthogonal
- **Eigenvalues**: Reveal scaling in each eigenvector direction
- **Stability**: Negative eigenvalues → stable system

---

## 3. Instructor Examples

### Example 1: Diagonal Matrix

**Question**: For A = [2, 0; 0, 3], what is the eigendecomposition?

**Solution**:
- Eigenvectors: [1, 0] and [0, 1]
- Eigenvalues: 2 and 3
- Q = [1, 0; 0, 1] (identity), Λ = [2, 0; 0, 3]
- A = Q·Λ·Q⁻¹ = I·Λ·I = Λ (already diagonal!)

**AI Connection**: Diagonal matrices are already in eigendecomposed form. This simplifies many calculations.

---

### Example 2: PCA Decomposition

**Question**: How does eigendecomposition relate to PCA?

**Solution**:
- Covariance matrix C is symmetric
- Eigendecomposition: C = Q·Λ·Qᵀ
- Q columns = principal components (eigenvectors)
- Λ diagonal = variances (eigenvalues)
- Project data onto top eigenvectors for dimensionality reduction

**AI Connection**: This is exactly how PCA works. Eigendecomposition reveals the most important directions in data.

---

### Example 3: Matrix Powers

**Question**: Why is A² easier with eigendecomposition?

**Solution**:
- A = Q·Λ·Q⁻¹
- A² = (Q·Λ·Q⁻¹)² = Q·Λ²·Q⁻¹
- Just square the eigenvalues (diagonal), keep eigenvectors
- Much easier than multiplying A by itself!

**AI Connection**: In some neural network architectures and optimization algorithms, we need matrix powers. Eigendecomposition makes this efficient.

---

## 4. Summary / Key Takeaways

- ✅ **Eigendecomposition**: A = Q·Λ·Q⁻¹ reveals matrix structure
- ✅ **PCA**: Uses eigendecomposition of covariance matrix
- ✅ **Efficiency**: Matrix powers easier with eigendecomposition
- ✅ **Symmetric matrices**: Always diagonalizable with orthogonal eigenvectors
- ✅ Eigendecomposition is fundamental to many advanced AI techniques

