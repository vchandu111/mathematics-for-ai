# Day 4 — Student Task: Definite Integrals

## Instructions

Evaluate the definite integrals using the Fundamental Theorem of Calculus. Show all steps: find the antiderivative, evaluate at both bounds, and subtract. Remember: no +C needed for definite integrals!

---

## Tasks

### Task 1: Basic Definite Integrals (Easy)

Evaluate:
- a) ∫[0 to 2] x² dx
- b) ∫[1 to 3] 2x dx
- c) ∫[0 to 4] x dx
- d) ∫[0 to 1] 3x² dx

**Expected Output**: Four numeric values with work shown (antiderivative, evaluation at bounds, final answer).

---

### Task 2: Basic Definite Integrals (Easy)

Evaluate:
- a) ∫[0 to 3] (x² + x) dx
- b) ∫[1 to 2] (2x² - x) dx
- c) ∫[0 to 2] (x³ - x) dx
- d) ∫[0 to 1] (4x² + 2x + 1) dx

**Expected Output**: Four numeric values with complete work shown.

---

### Task 3: Medium Reasoning Question

For the definite integral ∫[1 to 4] 3x² dx:

- a) Evaluate the integral
- b) What does this number represent geometrically?
- c) If this were a probability density function, what would this integral represent?

**Expected Output**: 
- Numeric value
- Written geometric interpretation
- Written probability interpretation

---

### Task 4: Application to AI (Medium)

A probability density function is f(x) = 6x(1-x) for 0 ≤ x ≤ 1.

- a) Verify that ∫[0 to 1] 6x(1-x) dx = 1 (expand first: 6x(1-x) = 6x - 6x²)
- b) Calculate P(0 ≤ X ≤ 0.5) = ∫[0 to 0.5] 6x(1-x) dx
- c) Calculate P(0.5 ≤ X ≤ 1) = ∫[0.5 to 1] 6x(1-x) dx
- d) Verify that the two probabilities sum to 1

**Expected Output**: 
- Verification calculation
- Two probability values
- Verification that they sum to 1

---

### Task 5: Medium Reasoning Question

Consider ∫[0 to 2] (x² - 2x) dx.

- a) Evaluate the integral
- b) Notice that the function is negative for some x values. How can an integral be negative? What does this mean?
- c) Calculate ∫[0 to 1] (x² - 2x) dx and ∫[1 to 2] (x² - 2x) dx separately. What do you observe?

**Expected Output**: 
- Three numeric values
- Written explanation of negative integrals
- Written observation about the split integrals

---

### Task 6: Expected Value Calculation (Medium)

For the probability density f(x) = 2x on [0, 1], calculate the expected value:

E[X] = ∫[0 to 1] x·f(x) dx = ∫[0 to 1] x·(2x) dx

- a) Set up and evaluate the integral
- b) What does this expected value tell us?
- c) Is this value reasonable given that X ranges from 0 to 1? Explain.

**Expected Output**: 
- Calculated expected value
- Written interpretation
- Written reasoning about reasonableness

---

### Task 7: Optional Python Task

Write a Python function to evaluate definite integrals:

```python
def definite_integral_power(n, a, b, coefficient=1):
    # Evaluate ∫[a to b] coefficient·xⁿ dx
    # Return the numeric value
```

Test with:
- ∫[0 to 3] x² dx (should be 9)
- ∫[1 to 2] 2x³ dx
- ∫[0 to 1] 3x² dx

**Expected Output**: Python code with function and test cases showing outputs.

---

## Expected Output / Answer Format

For each task, provide:
- **Numeric values**: Final answers for definite integrals
- **Work shown**: Antiderivative, evaluation at bounds, subtraction
- **Interpretations**: Written explanations of what the values mean
- **Verifications**: Check that probabilities sum correctly

**Note**: No solutions are provided—work through each problem independently!

