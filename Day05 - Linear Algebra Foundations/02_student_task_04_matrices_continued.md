# Day 5 — Student Task: Matrices Continued

## Instructions

Complete these matrix multiplication tasks. Show your work step-by-step, especially the dot products for each element.

---

## Tasks

### Task 1: Basic Matrix Multiplication (Easy)

Calculate:
- a) [1, 2] × [5; 6] (2×2 × 2×1)
- b) [1, 2; 3, 4] × [5, 6; 7, 8]
- c) [1, 2, 3] × [4; 5; 6] (1×3 × 3×1)

**Expected Output**: Three matrix products with work shown.

---

### Task 2: Dimension Checking (Easy)

Determine if these multiplications are possible. If yes, give dimensions of result:
- a) (2×3) × (3×4)
- b) (3×2) × (2×3)
- c) (2×3) × (2×3)
- d) (1×4) × (4×1)

**Expected Output**: Four answers (possible/not possible, and result dimensions if possible).

---

### Task 3: Medium Reasoning Question

Calculate A × B where:
- A = [1, 2; 3, 4]
- B = [5, 6; 7, 8]

- a) Calculate A × B
- b) Calculate B × A
- c) Are they the same? What does this tell us about matrix multiplication?
- d) Is matrix multiplication commutative?

**Expected Output**: 
- Two matrix products
- Comparison
- Written explanation

---

### Task 4: Application to AI (Medium)

A neural network layer:
- Input: x = [2; 3; 1] (3 features)
- Weights: W = [0.5, 0.3, 0.2; 0.1, 0.4, 0.6] (2 neurons, 3 inputs each)

- a) What are the dimensions of W × x?
- b) Calculate the output: W × x
- c) What does each element of the output represent?

**Expected Output**: 
- Dimension specification
- Calculated output vector
- Written explanation

---

### Task 5: Batch Processing (Medium)

Process a batch of 3 examples:
- Input matrix X = [1, 2; 3, 4; 5, 6] (3 examples, 2 features each)
- Weight matrix W = [0.5, 0.3; 0.2, 0.8] (2 inputs, 2 outputs)

- a) What are the dimensions of X × W?
- b) Calculate X × W
- c) What does each row of the result represent?

**Expected Output**: 
- Dimension specification
- Calculated output matrix
- Written explanation

---

### Task 6: Optional Python Task

Write Python code using numpy to multiply matrices:

```python
import numpy as np

def matrix_multiply(A, B):
    # Multiply matrices A and B
    return result
```

Test with examples from Task 1.

**Expected Output**: Python code with function and test cases.

---

## Expected Output / Answer Format

For each task, provide:
- **Matrix products**: Show final results
- **Work shown**: Step-by-step calculations for each element
- **Dimension analysis**: Check compatibility before multiplying
- **Written explanations**: Brief reasoning where requested

**Note**: No solutions are provided—work through each problem independently!

