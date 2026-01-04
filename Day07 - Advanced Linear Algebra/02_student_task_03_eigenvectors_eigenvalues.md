# Day 7 — Student Task: Eigenvectors & Eigenvalues

## Instructions

Work with eigenvectors and eigenvalues. Focus on understanding what they represent rather than complex calculations.

---

## Tasks

### Task 1: Verify Eigenvectors (Easy)

For matrix A = [3, 0; 0, 2]:
- a) Verify that [1, 0] is an eigenvector. What is its eigenvalue?
- b) Verify that [0, 1] is an eigenvector. What is its eigenvalue?
- c) Calculate A·[1, 0] and A·[0, 1] to verify.

**Expected Output**: 
- Two eigenvalue identifications
- Two verification calculations

---

### Task 2: Medium Reasoning Question

- a) What does it mean for a vector to be an eigenvector?
- b) What does the eigenvalue tell us about the transformation?
- c) Why might eigenvectors be useful in machine learning?

**Expected Output**: Written explanations for all three parts.

---

### Task 3: Application to AI (Medium)

In Principal Component Analysis:

- a) What matrix's eigenvectors do we find?
- b) What do the eigenvalues represent?
- c) Why do we typically keep eigenvectors with the largest eigenvalues?
- d) How does this relate to dimensionality reduction?

**Expected Output**: Written explanations for all four parts.

---

### Task 4: Optional Python Task

Use numpy to find eigenvectors and eigenvalues:

```python
import numpy as np

eigenvalues, eigenvectors = np.linalg.eig(matrix)
```

Test with A = [3, 0; 0, 2] and verify the results.

**Expected Output**: Python code with calculation and verification.

---

## Expected Output / Answer Format

For each task, provide:
- **Verifications**: Show A·v = λ·v
- **Eigenvalue identification**: Match eigenvalues to eigenvectors
- **Written explanations**: Clear reasoning about concepts
- **Code**: Python implementations where requested

**Note**: Focus on understanding concepts and AI applications!

