# Day 2 — Student Task: Derivatives Intuition

## Instructions

Complete these tasks to build intuition about derivatives. Focus on understanding what derivatives represent rather than complex calculations. Show your reasoning for each answer.

---

## Tasks

### Task 1: Understanding Rate of Change (Easy)

A function f(x) represents the position of an object over time. At x = 3, the derivative f'(3) = 5.

Answer:
- a) What does f'(3) = 5 mean in practical terms?
- b) If we increase x from 3 to 3.1, approximately how much does f(x) change?
- c) Is the function increasing or decreasing at x = 3?

**Expected Output**: Written explanations for all three parts.

---

### Task 2: Visual Interpretation (Easy)

Consider a function where:
- At x = 1, the derivative is positive
- At x = 2, the derivative is zero
- At x = 3, the derivative is negative

Answer:
- a) What is happening to the function at x = 1?
- b) What is happening to the function at x = 2?
- c) What is happening to the function at x = 3?
- d) Sketch a rough graph showing this behavior

**Expected Output**: Written explanations and a brief description or sketch of the graph.

---

### Task 3: Medium Reasoning Question

An AI model's loss function L(w) has the following derivatives at different weight values:
- At w = 0.5: L'(0.5) = -2
- At w = 1.0: L'(1.0) = 0
- At w = 1.5: L'(1.5) = 3

Answer:
- a) At which weight value is the loss decreasing fastest?
- b) At which weight value might we have found an optimal point?
- c) If we're at w = 0.5 and want to minimize loss, should we increase or decrease w? Why?
- d) If we're at w = 1.5 and want to minimize loss, should we increase or decrease w? Why?

**Expected Output**: Answers to all four parts with brief explanations.

---

### Task 4: Medium Reasoning Question

The derivative of f(x) = x² is f'(x) = 2x.

- a) Calculate f'(0), f'(1), f'(2), and f'(3)
- b) What pattern do you notice?
- c) As x increases, what happens to the rate of change? What does this mean for the function's behavior?
- d) At what x value is the derivative zero? What is special about this point?

**Expected Output**: 
- Table of derivative values
- Written explanations for parts (b), (c), and (d)

---

### Task 5: Application to AI (Medium)

In gradient descent, we update weights using: w_new = w_old - learning_rate × gradient

For a loss function L(w):
- At w = 2, the gradient (derivative) is L'(2) = 4
- Learning rate = 0.1

Answer:
- a) Calculate the new weight value after one gradient descent step
- b) Why do we subtract (learning_rate × gradient) instead of adding?
- c) If the learning rate were 0.5 instead of 0.1, what would the new weight be? Is this better or worse? Why?

**Expected Output**: 
- Numeric answer for part (a)
- Written explanations for parts (b) and (c)

---

### Task 6: Understanding Steepness (Medium)

Two functions have derivatives at the same point:
- Function A: f'(5) = 10
- Function B: g'(5) = 0.1

Answer:
- a) Which function is changing faster at x = 5?
- b) If these represent error functions in AI, which one would require a smaller learning rate? Why?
- c) What does a very large derivative value tell us about the function's behavior?

**Expected Output**: Written explanations for all three parts.

---

### Task 7: Optional Python Task

Write a Python function that approximates the derivative using the limit definition:

```python
def approximate_derivative(func, x, h=0.0001):
    # Calculate [f(x+h) - f(x)] / h
    # Return approximate derivative
```

Test with:
- f(x) = x² at x = 2 (should be close to 4)
- f(x) = 3x + 1 at x = 5 (should be close to 3)
- f(x) = x³ at x = 1 (should be close to 3)

**Expected Output**: Python code with function and test cases showing outputs.

---

## Expected Output / Answer Format

For each task, provide:
- **Numeric answers**: Where calculations are needed
- **Written explanations**: Clear reasoning for conceptual questions
- **Tables**: Use tables to organize multiple calculations
- **Sketches/Descriptions**: Brief descriptions of graphs or visual concepts

**Note**: No solutions are provided—work through each problem independently!

