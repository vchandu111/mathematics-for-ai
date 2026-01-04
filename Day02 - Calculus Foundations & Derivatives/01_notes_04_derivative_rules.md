# Day 2 — Derivative Rules

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Learn Basic Derivative Rules | Master power rule, constant rule, and sum rule |
| 2 | Apply Rules to Functions | Calculate derivatives of common functions |
| 3 | Use Rules in AI Context | See how these rules are applied in gradient calculations |

---

## 1. Introduction

### Why Derivative Rules?

Instead of using the limit definition every time, we have **rules** that make calculating derivatives much faster. These rules are like shortcuts that always work.

### Why These Rules Matter for AI

In AI, we need to calculate derivatives (gradients) for:
- **Loss functions**: Error functions that need optimization
- **Activation functions**: Functions used in neural network layers
- **Complex models**: Functions with many terms

Using rules makes these calculations efficient and practical.

### Real-World Analogy

Think of derivative rules like multiplication tables:
- You could calculate 7 × 8 by adding 7 eight times
- But it's much faster to just know 7 × 8 = 56
- Derivative rules are the "multiplication tables" of calculus!

---

## 2. Deep-Dive Explanation

### Rule 1: Power Rule

**Rule**: If f(x) = xⁿ, then f'(x) = n·xⁿ⁻¹

**Examples**:
- f(x) = x² → f'(x) = 2x
- f(x) = x³ → f'(x) = 3x²
- f(x) = x → f'(x) = 1 (since x = x¹)
- f(x) = 1/x = x⁻¹ → f'(x) = -x⁻² = -1/x²

### Rule 2: Constant Rule

**Rule**: If f(x) = c (constant), then f'(x) = 0

**Examples**:
- f(x) = 5 → f'(x) = 0
- f(x) = π → f'(x) = 0

**Intuition**: Constants don't change, so their rate of change is zero.

### Rule 3: Constant Multiple Rule

**Rule**: If f(x) = c·g(x), then f'(x) = c·g'(x)

**Examples**:
- f(x) = 3x² → f'(x) = 3·(2x) = 6x
- f(x) = -5x³ → f'(x) = -5·(3x²) = -15x²

### Rule 4: Sum/Difference Rule

**Rule**: If f(x) = g(x) ± h(x), then f'(x) = g'(x) ± h'(x)

**Examples**:
- f(x) = x² + 3x → f'(x) = 2x + 3
- f(x) = x³ - 2x → f'(x) = 3x² - 2

### Combining Rules

You can combine these rules for complex functions:

**Example**: f(x) = 4x³ - 2x² + 5x - 7
- f'(x) = 4·(3x²) - 2·(2x) + 5·(1) - 0
- f'(x) = 12x² - 4x + 5

---

## 3. Instructor Examples

### Example 1: Simple Power Rule

**Question**: What is the derivative of f(x) = x⁴?

**Solution**:
- Using power rule: f'(x) = 4·x⁴⁻¹ = 4x³

**AI Connection**: Many activation functions in neural networks use power functions. Knowing their derivatives helps calculate gradients efficiently.

---

### Example 2: Constant Multiple

**Question**: What is the derivative of f(x) = 5x²?

**Solution**:
- First, derivative of x² is 2x (power rule)
- Then multiply by constant: f'(x) = 5·(2x) = 10x

**AI Connection**: In neural networks, weights are often multiplied by constants. This rule helps us calculate how changing the weight affects the output.

---

### Example 3: Sum of Terms

**Question**: What is the derivative of f(x) = 3x² + 2x + 1?

**Solution**:
- Apply rules term by term:
  - Derivative of 3x² = 3·(2x) = 6x
  - Derivative of 2x = 2·(1) = 2
  - Derivative of 1 = 0
- f'(x) = 6x + 2

**AI Connection**: Loss functions in machine learning are often sums of multiple terms. This rule lets us calculate the gradient efficiently.

---

### Example 4: Complex Function

**Question**: What is the derivative of f(x) = 2x³ - 5x² + 3x - 10?

**Solution**:
- Apply rules to each term:
  - 2x³ → 2·(3x²) = 6x²
  - -5x² → -5·(2x) = -10x
  - 3x → 3·(1) = 3
  - -10 → 0
- f'(x) = 6x² - 10x + 3

**AI Connection**: This is exactly the type of calculation done in backpropagation. Each term's derivative is calculated separately, then combined.

---

### Example 5: AI Loss Function

**Question**: A simple loss function is L(w) = (w - 3)². What is L'(w)?

**Solution**:
- First expand: L(w) = (w - 3)² = w² - 6w + 9
- Apply derivative rules:
  - w² → 2w
  - -6w → -6
  - 9 → 0
- L'(w) = 2w - 6

**AI Connection**: This derivative tells us how to adjust weight w to minimize loss. When L'(w) = 0, we get 2w - 6 = 0, so w = 3 (the optimal value).

---

## 4. Summary / Key Takeaways

- ✅ **Power Rule**: f(x) = xⁿ → f'(x) = n·xⁿ⁻¹
- ✅ **Constant Rule**: f(x) = c → f'(x) = 0
- ✅ **Constant Multiple**: f(x) = c·g(x) → f'(x) = c·g'(x)
- ✅ **Sum/Difference Rule**: f(x) = g(x) ± h(x) → f'(x) = g'(x) ± h'(x)
- ✅ These rules make gradient calculation efficient in AI/ML
- ✅ Combine rules for complex functions by applying them term-by-term

