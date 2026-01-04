# Day 7 — Eigenvectors & Eigenvalues

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Eigenvectors | Learn vectors that don't change direction under transformation |
| 2 | Understand Eigenvalues | Learn the scaling factor for eigenvectors |
| 3 | Connect to AI | See how eigenvalues appear in PCA, SVD, and neural networks |

---

## 1. Introduction

### What are Eigenvectors and Eigenvalues?

For a matrix A, an **eigenvector** v is a special vector where:
**A·v = λ·v**

Where λ (lambda) is the **eigenvalue** (scaling factor).

**Key Insight**: Eigenvectors don't change direction when transformed by A, only scale by eigenvalue.

### Why Eigenvectors Matter for AI

- **PCA**: Principal components are eigenvectors of covariance matrix
- **SVD**: Singular value decomposition uses eigenvectors
- **Stability Analysis**: Eigenvalues indicate system stability
- **Dimensionality Reduction**: Keep eigenvectors with largest eigenvalues

---

## 2. Deep-Dive Explanation

### Definition

For matrix A and vector v:
- If A·v = λ·v, then:
  - v is an eigenvector
  - λ is the corresponding eigenvalue

### Finding Eigenvectors

Solve: (A - λI)·v = 0
- This gives characteristic equation
- Solve for eigenvalues λ
- For each λ, find corresponding eigenvector v

---

## 3. Instructor Examples

### Example 1: Simple Eigenvector

**Question**: For A = [2, 0; 0, 3], find eigenvectors and eigenvalues.

**Solution**:
- A·[1, 0] = [2, 0] = 2·[1, 0] → eigenvalue 2
- A·[0, 1] = [0, 3] = 3·[0, 1] → eigenvalue 3
- Eigenvectors: [1, 0] and [0, 1] (standard basis vectors)

**AI Connection**: Diagonal matrices have standard basis as eigenvectors. This simplifies many calculations.

---

### Example 2: PCA Connection

**Question**: Why are eigenvectors important in PCA?

**Solution**:
- Covariance matrix's eigenvectors = principal components
- Eigenvalues = variance along each component
- Larger eigenvalue = more important direction
- Keep top eigenvectors for dimensionality reduction

**AI Connection**: PCA finds eigenvectors of data covariance matrix. These directions capture most variance.

---

## 4. Summary / Key Takeaways

- ✅ **Eigenvector**: v where A·v = λ·v (direction unchanged by transformation)
- ✅ **Eigenvalue**: Scaling factor λ
- ✅ **PCA**: Uses eigenvectors of covariance matrix as principal components
- ✅ **Dimensionality Reduction**: Keep eigenvectors with largest eigenvalues
- ✅ Eigenvectors reveal the most important directions in data transformations

