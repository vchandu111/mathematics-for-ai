# Day 6 — Determinant

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Determinant | Learn what determinant measures (area/volume scaling) |
| 2 | Calculate Determinants | Master 2×2 and 3×3 determinants |
| 3 | Connect to AI | See how determinants indicate invertibility and volume changes |

---

## 1. Introduction

### What is Determinant?

The **determinant** of a matrix is a single number that tells us:
- **Scaling Factor**: How much area/volume is scaled by the transformation
- **Invertibility**: If det(A) = 0, matrix is not invertible
- **Orientation**: Sign tells us if orientation is flipped

### Why Determinant Matters for AI

- **Invertibility**: Need det ≠ 0 to have inverse (important for solving systems)
- **Volume Preservation**: Some transformations preserve volume (det = ±1)
- **Numerical Stability**: Very small determinants indicate near-singular matrices (problematic)

---

## 2. Deep-Dive Explanation

### 2×2 Determinant

For A = [a, b; c, d]:
**det(A) = ad - bc**

### 3×3 Determinant

For A = [a, b, c; d, e, f; g, h, i]:
**det(A) = a(ei - fh) - b(di - fg) + c(dh - eg)**

### Key Properties

- **det(A) = 0**: Matrix is singular (not invertible)
- **det(A) ≠ 0**: Matrix is invertible
- **det(I) = 1**: Identity matrix
- **det(AB) = det(A) × det(B)**: Determinant of product

---

## 3. Instructor Examples

### Example 1: 2×2 Determinant

**Question**: Calculate det([2, 3; 1, 4]).

**Solution**:
- det = 2×4 - 3×1 = 8 - 3 = 5
- Since det ≠ 0, matrix is invertible

**AI Connection**: Before inverting a matrix (solving linear systems), we check the determinant.

---

### Example 2: Singular Matrix

**Question**: Calculate det([1, 2; 2, 4]).

**Solution**:
- det = 1×4 - 2×2 = 4 - 4 = 0
- Matrix is singular (not invertible)

**AI Connection**: Singular matrices cause problems in optimization and solving systems. We need to detect and handle them.

---

### Example 3: Identity Matrix

**Question**: What is det(I) for 2×2 identity?

**Solution**:
- det([1, 0; 0, 1]) = 1×1 - 0×0 = 1
- Identity preserves area (scaling factor = 1)

**AI Connection**: Identity transformations preserve volume, which is useful in some neural network architectures.

---

## 4. Summary / Key Takeaways

- ✅ **Determinant**: Single number measuring area/volume scaling
- ✅ **2×2 formula**: det = ad - bc
- ✅ **det = 0**: Matrix is singular (not invertible)
- ✅ **det ≠ 0**: Matrix is invertible
- ✅ Used in AI to check invertibility and numerical stability

