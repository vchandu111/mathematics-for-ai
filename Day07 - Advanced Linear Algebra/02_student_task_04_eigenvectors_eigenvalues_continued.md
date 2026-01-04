# Day 7 — Student Task: Eigenvectors & Eigenvalues Continued

## Instructions

Explore eigendecomposition and its applications. Focus on understanding concepts and AI connections.

---

## Tasks

### Task 1: Understanding Decomposition (Medium)

- a) What does eigendecomposition A = Q·Λ·Q⁻¹ tell us about a matrix?
- b) What do the columns of Q represent?
- c) What do the diagonal elements of Λ represent?
- d) Why is this decomposition useful?

**Expected Output**: Written explanations for all four parts.

---

### Task 2: Application to PCA (Medium)

In Principal Component Analysis:

- a) What matrix do we decompose?
- b) What do the eigenvectors represent?
- c) What do the eigenvalues represent?
- d) How do we use this for dimensionality reduction?

**Expected Output**: Written explanations connecting eigendecomposition to PCA.

---

### Task 3: Medium Reasoning Question

- a) Why are symmetric matrices special in eigendecomposition?
- b) What does it mean if all eigenvalues are positive?
- c) What does it mean if an eigenvalue is zero?
- d) How might eigenvalues indicate numerical stability issues?

**Expected Output**: Written explanations for all four parts.

---

### Task 4: Optional Python Task

Use numpy to perform eigendecomposition:

```python
import numpy as np

eigenvalues, eigenvectors = np.linalg.eig(A)
# Reconstruct: A_reconstructed = eigenvectors @ np.diag(eigenvalues) @ np.linalg.inv(eigenvectors)
```

Test with a symmetric matrix and verify reconstruction.

**Expected Output**: Python code with eigendecomposition and verification.

---

## Expected Output / Answer Format

For each task, provide:
- **Written explanations**: Clear conceptual understanding
- **AI connections**: How eigendecomposition applies to ML
- **Code**: Python implementations where requested
- **Verifications**: Check reconstructions work correctly

**Note**: Focus on understanding the power and applications of eigendecomposition!

