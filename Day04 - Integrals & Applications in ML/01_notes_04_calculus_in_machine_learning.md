# Day 4 — Calculus in Machine Learning

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Gradient Descent | See how derivatives optimize neural networks |
| 2 | Understand Backpropagation | Learn how calculus enables learning |
| 3 | Connect All Concepts | See how probability, derivatives, and integrals work together in AI |

---

## 1. Introduction

### How Calculus Powers AI

Calculus is the mathematical engine behind how AI learns:

- **Gradient Descent**: Uses derivatives to find optimal parameters
- **Backpropagation**: Calculates gradients through the network using chain rule
- **Optimization**: Minimizes loss functions using derivatives
- **Probability**: Uses integrals for continuous distributions

### The Big Picture

Every time a neural network learns, it's using calculus:
1. **Forward Pass**: Calculate predictions
2. **Calculate Loss**: Measure error
3. **Backward Pass**: Calculate derivatives (gradients)
4. **Update Weights**: Move in direction that reduces error (gradient descent)

---

## 2. Deep-Dive Explanation

### Gradient Descent: The Core Algorithm

**Goal**: Minimize loss function L(w)

**Process**:
1. Calculate gradient: ∇L(w) = dL/dw
2. Update weight: w_new = w_old - α·∇L(w)
   - α = learning rate (how big steps to take)
   - Negative sign because we want to minimize (go downhill)

**Intuition**: The gradient points in the direction of steepest increase. We go opposite (negative) to decrease the loss.

### Backpropagation: Calculating Gradients

**Chain Rule**: If y = f(g(x)), then dy/dx = (dy/dg)·(dg/dx)

In neural networks:
- Output depends on hidden layers
- Hidden layers depend on inputs
- We chain derivatives backward through the network

### Visual Representation

```
Gradient Descent:
Loss
  │    ╱───╲
  │   ╱     ╲
  │  ╱       ╲
  │ ╱         ╲
  │╱           ╲
 ─┴──────────────┴─
        Weights

At each point, gradient tells us which way to go (downhill)
```

---

## 3. Instructor Examples

### Example 1: Simple Gradient Descent

**Question**: Loss function L(w) = w². Current weight w = 3. Learning rate α = 0.1. What's the new weight?

**Solution**:
- Gradient: L'(w) = 2w
- At w = 3: L'(3) = 6
- Update: w_new = 3 - 0.1·6 = 3 - 0.6 = 2.4
- The weight moved toward 0 (the minimum)!

**AI Connection**: This is exactly what happens in neural network training. Each weight gets updated based on its gradient.

---

### Example 2: Understanding the Learning Rate

**Question**: Same function L(w) = w², w = 3. What happens with α = 0.5 vs α = 0.01?

**Solution**:
- With α = 0.5: w_new = 3 - 0.5·6 = 0 (jumps to minimum, might overshoot)
- With α = 0.01: w_new = 3 - 0.01·6 = 2.94 (small step, slow but stable)

**AI Connection**: Learning rate is crucial. Too large = unstable training. Too small = very slow training.

---

### Example 3: Chain Rule in Backpropagation

**Question**: In a simple network: input x → weight w → output y = w·x. Loss L = (y - target)². Find dL/dw.

**Solution**:
- y = w·x
- L = (y - target)²
- Chain rule: dL/dw = (dL/dy)·(dy/dw)
- dL/dy = 2(y - target)
- dy/dw = x
- dL/dw = 2(y - target)·x

**AI Connection**: This is backpropagation! We calculate how loss changes with each weight by chaining derivatives.

---

### Example 4: Probability and Integration

**Question**: A model outputs probability scores. To get the probability that score is between 0.3 and 0.7, we integrate the probability density.

**Solution**:
- If PDF is f(x), then P(0.3 ≤ X ≤ 0.7) = ∫[0.3 to 0.7] f(x) dx
- This gives us the probability over that range

**AI Connection**: Many AI models output probability distributions. We use integrals to calculate probabilities for ranges of values.

---

### Example 5: Expected Value in AI

**Question**: Calculate the expected prediction score if the probability density is f(x) = 2x on [0, 1].

**Solution**:
- E[X] = ∫[0 to 1] x·f(x) dx = ∫[0 to 1] x·(2x) dx = ∫[0 to 1] 2x² dx
- = (2/3)x³|[0 to 1] = 2/3 - 0 = 2/3

**AI Connection**: Expected values tell us average model outputs, which helps understand model behavior and calibration.

---

## 4. Summary / Key Takeaways

- ✅ **Gradient Descent**: Uses derivatives to minimize loss: w_new = w_old - α·∇L
- ✅ **Backpropagation**: Uses chain rule to calculate gradients through networks
- ✅ **Learning Rate**: Controls step size in optimization (balance speed vs stability)
- ✅ **Probability**: Integrals calculate probabilities for continuous distributions
- ✅ **Expected Values**: Integrals of x·f(x) give average outcomes
- ✅ **All Connected**: Derivatives optimize, integrals calculate probabilities—calculus is everywhere in AI!

