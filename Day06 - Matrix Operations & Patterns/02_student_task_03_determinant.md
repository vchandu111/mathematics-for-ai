# Day 6 — Student Task: Determinant

## Instructions

Calculate determinants and understand their meaning. Show your work using the formulas.

---

## Tasks

### Task 1: 2×2 Determinants (Easy)

Calculate:
- a) det([1, 2; 3, 4])
- b) det([2, 1; 4, 2])
- c) det([5, 0; 0, 3])
- d) det([1, 0; 0, 1])

**Expected Output**: Four determinant values with work shown.

---

### Task 2: Singular Matrices (Easy)

- a) Calculate det([1, 2; 2, 4])
- b) Calculate det([3, 6; 1, 2])
- c) What do these determinants tell you about the matrices?
- d) Can these matrices be inverted? Why or why not?

**Expected Output**: 
- Two determinant values
- Written interpretation
- Invertibility determination

---

### Task 3: Medium Reasoning Question

For matrices:
- A = [2, 1; 3, 4]
- B = [1, 0; 0, 2]

- a) Calculate det(A)
- b) Calculate det(B)
- c) Calculate det(A × B)
- d) Verify that det(A × B) = det(A) × det(B)

**Expected Output**: 
- Three determinant values
- Verification of property

---

### Task 4: Application to AI (Medium)

In solving linear systems Ax = b, we need A to be invertible.

- a) For A = [1, 2; 3, 6], calculate det(A)
- b) Can we solve Ax = b for this matrix? Explain.
- c) What does a very small determinant (near zero) indicate in numerical computations?
- d) Why is this important in neural network training?

**Expected Output**: 
- Determinant value
- Written explanation
- Written interpretation
- AI connection explanation

---

### Task 5: Optional Python Task

Write Python code to calculate 2×2 determinants:

```python
import numpy as np

def determinant_2x2(matrix):
    # Calculate determinant of 2×2 matrix
    return result
```

Test with examples from Task 1.

**Expected Output**: Python code with function and test cases.

---

## Expected Output / Answer Format

For each task, provide:
- **Determinant values**: Numeric results
- **Work shown**: Step-by-step using formulas
- **Interpretations**: What determinants tell us
- **Verifications**: Check properties where requested

**Note**: No solutions are provided—work through each problem independently!

