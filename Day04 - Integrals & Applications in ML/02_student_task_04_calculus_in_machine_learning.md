# Day 4 — Student Task: Calculus in Machine Learning

## Instructions

Complete these tasks connecting calculus concepts to machine learning. Show your work and explain how each concept applies to AI.

---

## Tasks

### Task 1: Basic Gradient Descent (Easy)

A simple loss function is L(w) = w² - 4w + 4, where w is a weight.

- a) Calculate L'(w) (the gradient)
- b) Find the value of w where L'(w) = 0 (optimal point)
- c) If current weight is w = 5 and learning rate α = 0.1, calculate the new weight after one gradient descent step
- d) Is the new weight closer to or farther from the optimal point?

**Expected Output**: 
- Gradient expression
- Optimal w value
- New weight after update
- Written explanation

---

### Task 2: Understanding Learning Rate (Easy)

For L(w) = w², current weight w = 4:

- a) Calculate the gradient at w = 4
- b) If learning rate α = 0.2, what is the new weight?
- c) If learning rate α = 0.01, what is the new weight?
- d) Which learning rate gets you closer to the minimum (w = 0) in one step? What are the trade-offs?

**Expected Output**: 
- Gradient value
- Two new weight values
- Written comparison and trade-off analysis

---

### Task 3: Medium Reasoning Question

In a neural network, the loss depends on output y, and output depends on weight w:
- y = 3w (simple linear relationship)
- L = (y - 6)² (loss function, target is 6)

- a) Use the chain rule to find dL/dw
- b) If w = 1, what is the gradient?
- c) With learning rate α = 0.1, what is the new weight?
- d) Explain how this demonstrates backpropagation

**Expected Output**: 
- Gradient expression using chain rule
- Numeric gradient value
- New weight value
- Written explanation

---

### Task 4: Application to AI (Medium)

A probability density function for model confidence scores is f(x) = 3x² on [0, 1].

- a) Verify this is a valid PDF (integrates to 1)
- b) Calculate P(confidence ≥ 0.7) = ∫[0.7 to 1] 3x² dx
- c) Calculate the expected confidence score E[X] = ∫[0 to 1] x·3x² dx
- d) What do these values tell us about the model's confidence distribution?

**Expected Output**: 
- Verification calculation
- Probability value
- Expected value
- Written interpretation

---

### Task 5: Medium Reasoning Question

Consider a loss function L(w) = w⁴ - 4w² + 4.

- a) Calculate L'(w)
- b) Find all w values where L'(w) = 0
- c) Which of these are minima? (Hint: check second derivative or test nearby points)
- d) Why might gradient descent get stuck at a local minimum instead of the global minimum?

**Expected Output**: 
- Derivative expression
- Critical points
- Identification of minima
- Written explanation of local vs global minima

---

### Task 6: Chain Rule Application (Medium)

In a two-layer network:
- Layer 1: h = 2x (x is input)
- Layer 2: y = 3h (h is hidden layer output)
- Loss: L = (y - 12)²

- a) Find dL/dh using chain rule
- b) Find dL/dx using chain rule (chain through both layers)
- c) If x = 1, what are the gradients?
- d) Explain how this shows gradients flowing backward through the network

**Expected Output**: 
- Two gradient expressions
- Numeric gradient values
- Written explanation of backpropagation

---

### Task 7: Integration in ML (Medium)

A model's prediction error follows a probability density f(e) = 2e on [0, 1], where e is the error.

- a) Verify this is a valid PDF
- b) Calculate P(error ≤ 0.5)
- c) Calculate the expected error E[E] = ∫[0 to 1] e·2e de
- d) What does a high expected error tell us about the model?

**Expected Output**: 
- Verification
- Probability value
- Expected error
- Written interpretation

---

### Task 8: Optional Python Task

Write Python code to simulate gradient descent for L(w) = w²:

```python
def gradient_descent(initial_w, learning_rate, iterations):
    w = initial_w
    for i in range(iterations):
        gradient = 2 * w  # derivative of w²
        w = w - learning_rate * gradient
        print(f"Iteration {i}: w = {w:.4f}")
    return w
```

Test with:
- initial_w = 5, learning_rate = 0.1, iterations = 10
- initial_w = 5, learning_rate = 0.5, iterations = 10

Compare the results.

**Expected Output**: Python code with function and test cases showing convergence.

---

## Expected Output / Answer Format

For each task, provide:
- **Calculations**: Show all derivative and integral work
- **Numeric values**: Final answers where requested
- **Written explanations**: Clear connections to AI/ML concepts
- **Code**: Python implementations where requested

**Note**: Focus on understanding how calculus concepts directly apply to machine learning!

