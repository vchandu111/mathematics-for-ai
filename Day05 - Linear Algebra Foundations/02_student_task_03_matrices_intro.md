# Day 5 — Student Task: Matrices Intro

## Instructions

Complete these tasks about basic matrix operations. Show your work clearly for addition and scalar multiplication.

---

## Tasks

### Task 1: Matrix Dimensions (Easy)

Identify the dimensions of each matrix:
- a) [1, 2; 3, 4]
- b) [1, 2, 3; 4, 5, 6]
- c) [1; 2; 3]
- d) [1, 2, 3, 4]

**Expected Output**: Four dimension specifications (m×n format).

---

### Task 2: Matrix Addition (Easy)

Calculate:
- a) [1, 2; 3, 4] + [5, 6; 7, 8]
- b) [1, 0; 0, 1] + [2, 3; 4, 5]
- c) [1, 2, 3] + [4, 5, 6] (if possible)
- d) [1, 2; 3, 4] + [1, 2, 3; 4, 5, 6] (if possible)

**Expected Output**: Matrix sums or explanation if addition is not possible.

---

### Task 3: Scalar Multiplication (Easy)

Calculate:
- a) 2 × [1, 2; 3, 4]
- b) -3 × [2, 0; 1, -1]
- c) 0.5 × [4, 6; 8, 10]
- d) 0 × [1, 2; 3, 4]

**Expected Output**: Four scaled matrices.

---

### Task 4: Medium Reasoning Question

Consider matrices:
- A = [1, 2; 3, 4]
- B = [5, 6; 7, 8]

- a) Calculate A + B
- b) Calculate 2A
- c) Calculate 2A + B
- d) Is matrix addition commutative? (Does A + B = B + A?) Verify.

**Expected Output**: 
- Three calculated matrices
- Verification of commutativity

---

### Task 5: Application to AI (Medium)

In a neural network, weight updates use: W_new = W_old - α·G, where:
- W_old = [0.5, 0.3; 0.2, 0.8] (old weights)
- G = [0.1, 0.05; 0.02, 0.1] (gradients)
- α = 0.1 (learning rate)

- a) Calculate α·G
- b) Calculate W_new
- c) What does this update represent in terms of learning?

**Expected Output**: 
- Scaled gradient matrix
- New weight matrix
- Written explanation

---

### Task 6: Medium Reasoning Question

A data matrix has 100 rows (examples) and 784 columns (features).

- a) What are the dimensions of this matrix?
- b) If each row represents one image, how many pixels does each image have?
- c) If we have a weight matrix W that transforms this data, and W is 784×128, what are the dimensions of the output?

**Expected Output**: 
- Matrix dimensions
- Number of pixels
- Output dimensions with explanation

---

### Task 7: Optional Python Task

Write Python code using numpy to:
- Create matrices
- Add matrices
- Multiply matrices by scalars

Test with the examples from Tasks 2 and 3.

**Expected Output**: Python code with operations and test cases.

---

## Expected Output / Answer Format

For each task, provide:
- **Matrix results**: Show final matrices clearly
- **Work shown**: Step-by-step calculations
- **Written explanations**: Brief reasoning where requested
- **Code**: Python implementations where requested

**Note**: No solutions are provided—work through each problem independently!

