# Day 2 — Student Task: Limits

## Instructions

Solve the following limit problems. For each problem, show your work and explain your reasoning. Remember that limits are about approaching values, not necessarily reaching them.

---

## Tasks

### Task 1: Basic Limit (Easy)

Calculate the following limits:
- a) lim(x→5) (3x + 2)
- b) lim(x→0) 7
- c) lim(x→-1) (x² + 3x - 1)

**Expected Output**: Three limit values with brief explanations.

---

### Task 2: Basic Limit (Easy)

Calculate:
- a) lim(x→4) (x² - 16) / (x - 4)
- b) lim(x→3) (x² - 9) / (x - 3)

**Hint**: You may need to factor and simplify first.

**Expected Output**: Two limit values with your simplification steps shown.

---

### Task 3: Medium Reasoning Question

Consider the function f(x) = (x² - 1) / (x - 1).

- a) What is f(1)? (Can you calculate it directly?)
- b) What is lim(x→1) f(x)? (Show your work)
- c) Explain why the answers to (a) and (b) are different. What does this teach us about limits?

**Expected Output**: 
- Answer to part (a)
- Answer to part (b) with calculation
- Written explanation for part (c)

---

### Task 4: Medium Reasoning Question

A neural network's error function behaves like: E(h) = (h² + 2h) / h, where h represents a small change.

- a) What happens to E(h) when h = 0? (Can you calculate it?)
- b) What is lim(h→0) E(h)?
- c) Why is understanding this limit important for gradient calculation in AI?

**Expected Output**: 
- Answer to part (a)
- Answer to part (b) with calculation
- Written explanation connecting to AI for part (c)

---

### Task 5: Application to AI (Medium)

The derivative (gradient) of a function f(x) at point a is defined as:

lim(h→0) [f(a+h) - f(a)] / h

For the function f(x) = x²:
- a) Write out the expression for the derivative at x = 3 using the limit definition
- b) Simplify the expression [f(3+h) - f(3)] / h
- c) Calculate lim(h→0) of your simplified expression
- d) What does this result represent in the context of AI optimization?

**Expected Output**: 
- Expression for part (a)
- Simplified expression for part (b)
- Limit value for part (c)
- Written explanation for part (d)

---

### Task 6: Understanding Behavior (Medium)

Consider f(x) = 1/x.

- a) What is lim(x→0⁺) f(x)? (approaching 0 from the positive side)
- b) What is lim(x→0⁻) f(x)? (approaching 0 from the negative side)
- c) Does lim(x→0) f(x) exist? Explain.
- d) Why is this important to understand when working with AI loss functions?

**Expected Output**: 
- Answers to parts (a) and (b)
- Written explanation for parts (c) and (d)

---

### Task 7: Optional Python Task

Write a Python function that approximates a limit by evaluating the function at values very close to the target point:

```python
def approximate_limit(func, target, direction='both'):
    # func: a function
    # target: the point we're approaching
    # direction: 'both', 'left', or 'right'
    # Return approximate limit value
```

Test with:
- f(x) = x², target = 2
- f(x) = (x² - 4)/(x - 2), target = 2

**Expected Output**: Python code with function and test cases showing outputs.

---

## Expected Output / Answer Format

For each task, provide:
- **Calculations**: Show all steps clearly
- **Simplifications**: Show factoring and algebraic manipulation
- **Final answers**: Numeric limit values
- **Explanations**: Brief reasoning, especially for AI connections

**Note**: No solutions are provided—work through each problem independently!

