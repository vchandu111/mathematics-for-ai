# Day 3 — Student Task: Integral Intuition

## Instructions

Complete these tasks to build intuition about integrals. Focus on understanding what integrals represent (accumulation, area) rather than complex calculations. Use geometric intuition where helpful.

---

## Tasks

### Task 1: Basic Area Interpretation (Easy)

For each function, describe what the integral ∫[a to b] f(x) dx represents:

- a) f(x) = 5 (constant function) from x = 0 to x = 3
- b) f(x) = x (linear function) from x = 0 to x = 4
- c) f(x) = 2x (linear function) from x = 1 to x = 3

**Expected Output**: Written descriptions of what each integral represents (you may calculate the areas if helpful).

---

### Task 2: Basic Accumulation (Easy)

A car's velocity (in m/s) over time is: v(t) = 2t, where t is in seconds.

- a) What is the velocity at t = 0? At t = 3?
- b) What does the integral ∫[0 to 3] 2t dt represent?
- c) Calculate this integral (hint: what shape does this form? What's its area?)

**Expected Output**: 
- Two velocity values
- Written explanation of what the integral represents
- Calculated area/distance

---

### Task 3: Medium Reasoning Question

Consider the function f(x) = x² from x = 0 to x = 2.

- a) Sketch or describe what the area under this curve looks like
- b) Is the area more or less than the area of a rectangle with width 2 and height 4? Explain.
- c) What does ∫[0 to 2] x² dx represent in practical terms?

**Expected Output**: 
- Description or sketch
- Comparison with rectangle
- Written explanation

---

### Task 4: Medium Reasoning Question

A probability density function is f(x) = 3x² for 0 ≤ x ≤ 1.

- a) What must be true about ∫[0 to 1] 3x² dx for this to be a valid probability distribution?
- b) Calculate ∫[0 to 1] 3x² dx (hint: antiderivative of x² is x³/3)
- c) Does your answer satisfy the requirement from part (a)? If not, what should the function be?

**Expected Output**: 
- Written requirement
- Calculated integral value
- Verification and correction if needed

---

### Task 5: Application to AI (Medium)

In machine learning, we often work with probability distributions. For a continuous random variable with density f(x) = 2x on [0, 1]:

- a) Verify that ∫[0 to 1] 2x dx = 1 (this ensures it's a valid probability distribution)
- b) What does the integral ∫[0 to 0.5] 2x dx represent?
- c) Calculate ∫[0 to 0.5] 2x dx
- d) What does this probability value tell us?

**Expected Output**: 
- Verification calculation
- Written explanation
- Calculated probability
- Interpretation

---

### Task 6: Understanding the Relationship (Medium)

Consider f(x) = x².

- a) What is the derivative of f(x)? (f'(x) = ?)
- b) What is an antiderivative of 2x? (∫ 2x dx = ?)
- c) What relationship do you notice between your answers to (a) and (b)?
- d) How does this demonstrate that integrals and derivatives are "opposites"?

**Expected Output**: 
- Derivative expression
- Antiderivative expression
- Written observation
- Written explanation of the relationship

---

### Task 7: Optional Python Task

Write a Python function that approximates the integral using rectangles (Riemann sum):

```python
def approximate_integral(func, a, b, n=1000):
    # Approximate ∫[a to b] f(x) dx using n rectangles
    # Return approximate area
```

Test with:
- f(x) = x from 0 to 4 (should be close to 8)
- f(x) = x² from 0 to 2 (should be close to 8/3)

**Expected Output**: Python code with function and test cases showing outputs.

---

## Expected Output / Answer Format

For each task, provide:
- **Calculations**: Show your work for any integrals you compute
- **Written explanations**: Clear descriptions of what integrals represent
- **Geometric intuition**: Use shapes and areas where helpful
- **Verifications**: Check that probability distributions integrate to 1

**Note**: No solutions are provided—work through each problem independently!

