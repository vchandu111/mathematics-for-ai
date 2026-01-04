# Day 5 — Student Task: Linear Transformations

## Instructions

Complete these tasks about linear transformations. You'll work with 2×2 matrices transforming 2D vectors. Show your matrix-vector multiplications step by step.

---

## Tasks

### Task 1: Basic Matrix-Vector Multiplication (Easy)

Apply these transformations to vector v = [2, 3]:

- a) A = [2, 0; 0, 2] (scaling matrix)
- b) B = [1, 0; 0, -1] (reflection across x-axis)
- c) C = [0, -1; 1, 0] (90° rotation)
- d) D = [-1, 0; 0, 1] (reflection across y-axis)

**Expected Output**: Four transformed vectors with work shown.

---

### Task 2: Understanding Effects (Easy)

For each matrix, describe what transformation it performs:

- a) [3, 0; 0, 3]
- b) [1, 0; 0, 0]
- c) [0, 1; 1, 0]
- d) [2, 0; 0, 1]

**Expected Output**: Written descriptions of each transformation.

---

### Task 3: Medium Reasoning Question

Apply transformation A = [2, 1; 0, 1] to vectors:
- u = [1, 0]
- v = [0, 1]
- w = [1, 1]

- a) Calculate A·u, A·v, and A·w
- b) Calculate A·(u + v) and compare with A·u + A·v
- c) What property does this demonstrate about linear transformations?

**Expected Output**: 
- Three transformed vectors
- Comparison showing linearity property
- Written explanation

---

### Task 4: Application to AI (Medium)

In a neural network, a layer applies transformation W to input x:
- W = [0.5, 0.3; 0.2, 0.8]
- Input x = [1, 1]

- a) Calculate the output: W·x
- b) If we double the input to [2, 2], what is the output?
- c) Compare 2·(W·x) with W·(2·x). What does this tell us?
- d) Why is linearity important in neural networks?

**Expected Output**: 
- Two output calculations
- Comparison
- Written explanation

---

### Task 5: Medium Reasoning Question

Consider transformations:
- A = [1, 0; 0, 2] (scales y by 2)
- B = [2, 0; 0, 1] (scales x by 2)

- a) Apply A to [1, 1], then B to the result
- b) Apply B to [1, 1], then A to the result
- c) Are the results the same? What does this tell us about order of transformations?
- d) Calculate B·A (matrix multiplication). What does this represent?

**Expected Output**: 
- Two transformation sequences
- Comparison
- Matrix product
- Written explanation

---

### Task 6: Optional Python Task

Write Python code to apply linear transformations:

```python
import numpy as np

def apply_transformation(matrix, vector):
    # Apply matrix transformation to vector
    return result
```

Test with:
- Matrix [2, 0; 0, 2] and vector [1, 1]
- Matrix [0, -1; 1, 0] and vector [2, 0]

**Expected Output**: Python code with function and test cases.

---

## Expected Output / Answer Format

For each task, provide:
- **Matrix-vector products**: Show calculation steps
- **Transformed vectors**: Final results
- **Written explanations**: Descriptions and reasoning
- **Comparisons**: Where asked, compare different approaches

**Note**: No solutions are provided—work through each problem independently!

