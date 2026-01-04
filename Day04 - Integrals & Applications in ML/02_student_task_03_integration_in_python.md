# Day 4 — Student Task: Integration in Python

## Instructions

Complete these Python integration tasks. You'll need to import `scipy.integrate` and `numpy`. Write Python code to solve each problem and show the output.

---

## Tasks

### Task 1: Basic Integration (Easy)

Write Python code to calculate:
- a) ∫[0 to 2] x² dx
- b) ∫[1 to 3] 2x dx
- c) ∫[0 to 4] x dx

**Expected Output**: Python code with three integration calculations and their outputs.

---

### Task 2: Probability Calculation (Easy)

A probability density function is f(x) = 3x² on [0, 1].

Write Python code to:
- a) Verify that ∫[0 to 1] 3x² dx = 1
- b) Calculate P(0 ≤ X ≤ 0.5)
- c) Calculate P(0.5 ≤ X ≤ 1)

**Expected Output**: Python code with verification and two probability calculations.

---

### Task 3: Medium Reasoning Question

For the function f(x) = x² + 2x + 1 on [0, 2]:

- a) Write Python code to calculate ∫[0 to 2] (x² + 2x + 1) dx
- b) Compare your Python result with the analytical answer (calculate by hand)
- c) What is the estimated error from Python? Is it acceptable?

**Expected Output**: 
- Python code and output
- Hand calculation
- Error analysis

---

### Task 4: Application to AI (Medium)

In machine learning, we often calculate expected values. For f(x) = 4x³ on [0, 1]:

- a) Verify it's a valid PDF (integrates to 1)
- b) Calculate E[X] = ∫[0 to 1] x·f(x) dx using Python
- c) What does this expected value represent in the context of AI?

**Expected Output**: 
- Python code for verification
- Python code for expected value
- Written explanation

---

### Task 5: Complex Function (Medium)

Calculate ∫[0 to 1] e⁻ˣ dx using Python.

- a) Write the Python code
- b) What is the result?
- c) Why might we need Python for this instead of calculating by hand?

**Expected Output**: 
- Python code
- Numeric result
- Written explanation

---

### Task 6: Custom Function (Medium)

Create a Python function that takes a function, lower bound, and upper bound, and returns the definite integral:

```python
def calculate_integral(func, a, b):
    # Your code here
    return result, error
```

Test it with:
- f(x) = x² from 0 to 3
- f(x) = 2x + 1 from 1 to 4

**Expected Output**: Python code with function definition and test cases.

---

### Task 7: Optional Advanced Task

Write a Python function that approximates the integral using the rectangle method (Riemann sum) and compare it with `scipy.integrate.quad`:

```python
def riemann_sum(func, a, b, n=1000):
    # Approximate using n rectangles
    # Return approximate value
```

Test with f(x) = x² from 0 to 2 and compare with the analytical answer (8/3).

**Expected Output**: Python code with both methods and comparison.

---

## Expected Output / Answer Format

For each task, provide:
- **Python code**: Complete, runnable code
- **Output**: Show the printed results
- **Comments**: Explain what your code does
- **Comparisons**: Where asked, compare Python results with analytical answers

**Note**: Make sure to import necessary libraries: `from scipy.integrate import quad` and `import numpy as np`

