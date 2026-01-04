# Day 7 — Student Task: Vector Calculus

## Instructions

Calculate gradients of multivariable functions. Show your partial derivatives clearly.

---

## Tasks

### Task 1: Basic Gradients (Easy)

Calculate gradients:
- a) f(x, y) = x + y
- b) f(x, y) = x² + y²
- c) f(x, y) = 2x + 3y
- d) f(x, y) = xy

**Expected Output**: Four gradient vectors with work shown.

---

### Task 2: Gradient at Points (Easy)

For f(x, y) = x² + y²:
- a) Calculate ∇f
- b) Evaluate ∇f at (1, 1)
- c) Evaluate ∇f at (0, 0)
- d) Evaluate ∇f at (2, 3)

**Expected Output**: 
- Gradient expression
- Three gradient vectors at specific points

---

### Task 3: Medium Reasoning Question

For f(x, y) = x² + 2xy + y²:

- a) Calculate ∇f
- b) At point (1, 1), what is the gradient?
- c) In which direction should we move to increase f fastest?
- d) In which direction should we move to decrease f fastest?

**Expected Output**: 
- Gradient expression
- Gradient at point
- Two direction vectors with explanations

---

### Task 4: Application to AI (Medium)

A loss function is L(w₁, w₂) = w₁² + w₂² - 4w₁ - 6w₂.

- a) Calculate ∇L
- b) At weights (2, 3), what is the gradient?
- c) If learning rate α = 0.1, calculate the weight update: w_new = w_old - α·∇L
- d) Are the new weights closer to or farther from the minimum? (Hint: minimum is where gradient = 0)

**Expected Output**: 
- Gradient expression
- Gradient at point
- Updated weights
- Written analysis

---

### Task 5: Optional Python Task

Write Python code to calculate gradients numerically:

```python
def gradient(f, x, y, h=0.0001):
    # Calculate gradient using finite differences
    return [df_dx, df_dy]
```

Test with f(x, y) = x² + y² at point (1, 1).

**Expected Output**: Python code with function and test case.

---

## Expected Output / Answer Format

For each task, provide:
- **Gradient expressions**: Vector of partial derivatives
- **Gradient values**: Evaluated at specific points
- **Work shown**: All partial derivative calculations
- **Interpretations**: Directions and meanings

**Note**: No solutions are provided—work through each problem independently!

