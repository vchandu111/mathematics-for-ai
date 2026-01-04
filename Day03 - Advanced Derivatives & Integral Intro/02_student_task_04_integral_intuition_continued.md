# Day 3 — Student Task: Integral Intuition Continued

## Instructions

Use the integration rules (power rule, constant multiple, sum rule) to find antiderivatives and evaluate definite integrals. Show your work clearly, including the constant of integration (+C) for indefinite integrals.

---

## Tasks

### Task 1: Basic Power Rule (Easy)

Find the antiderivatives:
- a) ∫ x⁴ dx
- b) ∫ x⁵ dx
- c) ∫ x dx
- d) ∫ 1 dx (hint: 1 = x⁰)

**Expected Output**: Four antiderivative expressions, each with +C.

---

### Task 2: Constant Multiple Rule (Easy)

Find the antiderivatives:
- a) ∫ 5x³ dx
- b) ∫ -3x² dx
- c) ∫ (1/2)x⁴ dx
- d) ∫ 7x dx

**Expected Output**: Four antiderivative expressions with work shown.

---

### Task 3: Sum Rule (Easy)

Find the antiderivatives:
- a) ∫ (x² + x) dx
- b) ∫ (x³ - x²) dx
- c) ∫ (2x² + 3x + 1) dx
- d) ∫ (x⁴ - 2x² + 5) dx

**Expected Output**: Four antiderivative expressions showing how you applied the sum rule.

---

### Task 4: Definite Integrals (Medium)

Evaluate the definite integrals:
- a) ∫[0 to 3] x² dx
- b) ∫[1 to 2] 2x dx
- c) ∫[0 to 1] (x² + x) dx
- d) ∫[0 to 2] 3x² dx

**Expected Output**: Four numeric values with work shown (antiderivative, evaluation at bounds, final answer).

---

### Task 5: Application to AI (Medium)

A probability density function is f(x) = 4x³ for 0 ≤ x ≤ 1.

- a) Verify that ∫[0 to 1] 4x³ dx = 1 (this ensures it's a valid probability distribution)
- b) Calculate P(0 ≤ X ≤ 0.5) = ∫[0 to 0.5] 4x³ dx
- c) Calculate P(0.5 ≤ X ≤ 1) = ∫[0.5 to 1] 4x³ dx
- d) Verify that P(0 ≤ X ≤ 0.5) + P(0.5 ≤ X ≤ 1) = 1

**Expected Output**: 
- Verification calculation
- Two probability values
- Verification that they sum to 1

---

### Task 6: Medium Reasoning Question

Consider ∫ (3x² + 2x - 1) dx.

- a) Find the antiderivative
- b) Verify your answer by taking the derivative of your result
- c) Why is it important to verify antiderivatives in AI applications?

**Expected Output**: 
- Antiderivative expression
- Derivative of your answer
- Written explanation

---

### Task 7: Combining All Rules (Medium)

Find the antiderivatives:
- a) ∫ (4x³ - 3x² + 2x - 5) dx
- b) ∫ (x⁴ - 2x³ + x²) dx
- c) ∫ (5x² - 3x + 7) dx

Then evaluate:
- d) ∫[0 to 2] (x² + 2x) dx
- e) ∫[1 to 3] (2x² - x) dx

**Expected Output**: 
- Three antiderivative expressions
- Two definite integral values

---

### Task 8: Optional Python Task

Write Python functions to:
- Calculate antiderivative using power rule: `antiderivative_power(n, coefficient=1)`
- Evaluate definite integral: `definite_integral_power(n, a, b, coefficient=1)`

Test with:
- ∫ x² dx (indefinite)
- ∫[0 to 3] x² dx (definite, should be 9)
- ∫[1 to 2] 2x³ dx (definite)

**Expected Output**: Python code with functions and test cases showing outputs.

---

## Expected Output / Answer Format

For each task, provide:
- **Antiderivative expressions**: Include +C for indefinite integrals
- **Work shown**: Show which rules you're applying
- **Definite integral values**: Show evaluation at bounds
- **Verifications**: Check your work by taking derivatives or summing probabilities

**Note**: No solutions are provided—work through each problem independently!

