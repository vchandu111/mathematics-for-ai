# Day 3 — Integral Intuition Continued

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Antiderivatives | Learn how to find functions whose derivative is given |
| 2 | Learn Basic Integration Rules | Master power rule for integrals and constant rules |
| 3 | Apply to Continuous Sums | See how integrals approximate sums of infinitely many terms |

---

## 1. Introduction

### What are Antiderivatives?

An **antiderivative** is the opposite of a derivative:
- If f'(x) = 2x, then an antiderivative of 2x is x²
- We write: ∫ 2x dx = x² + C (the +C is the constant of integration)

### Why Antiderivatives Matter for AI

Finding antiderivatives helps us:

- **Calculate Areas**: Find total probability, expected values
- **Solve Differential Equations**: Model how systems evolve over time
- **Optimization**: Understand total effects of changes
- **Continuous Models**: Work with continuous probability distributions

### Real-World Analogy

Think of antiderivatives like "reverse engineering":
- **Derivative**: "I have a recipe, what are the ingredients?" (breaking down)
- **Antiderivative**: "I have ingredients, what recipe could make this?" (building up)

In AI: We often know rates of change (derivatives) and need to find the original functions (antiderivatives).

---

## 2. Deep-Dive Explanation

### The Power Rule for Integrals

**Rule**: ∫ xⁿ dx = xⁿ⁺¹/(n+1) + C (where n ≠ -1)

**Examples**:
- ∫ x dx = x²/2 + C
- ∫ x² dx = x³/3 + C
- ∫ x³ dx = x⁴/4 + C

**Note**: The +C is called the "constant of integration" because the derivative of any constant is 0.

### Constant Rules

1. **Constant Multiple**: ∫ c·f(x) dx = c·∫ f(x) dx
2. **Sum Rule**: ∫ [f(x) + g(x)] dx = ∫ f(x) dx + ∫ g(x) dx

### Examples

- ∫ 5x² dx = 5·∫ x² dx = 5·(x³/3) + C = (5x³/3) + C
- ∫ (x² + x) dx = ∫ x² dx + ∫ x dx = x³/3 + x²/2 + C

### Why the Constant C?

When we differentiate x² + 5, we get 2x.
When we differentiate x² + 100, we get 2x.
Both are antiderivatives of 2x!

So: ∫ 2x dx = x² + C (where C can be any constant)

---

## 3. Instructor Examples

### Example 1: Simple Power Rule

**Question**: What is ∫ x³ dx?

**Solution**:
- Using power rule: ∫ x³ dx = x³⁺¹/(3+1) + C = x⁴/4 + C

**AI Connection**: In probability calculations, we often integrate polynomial functions. This rule makes it straightforward.

---

### Example 2: Constant Multiple

**Question**: What is ∫ 4x² dx?

**Solution**:
- Factor out constant: 4·∫ x² dx
- Apply power rule: 4·(x³/3) + C
- = (4x³/3) + C

**AI Connection**: Loss functions often have constant multipliers. This rule helps us integrate them efficiently.

---

### Example 3: Sum of Terms

**Question**: What is ∫ (2x² + 3x + 1) dx?

**Solution**:
- Split into separate integrals: ∫ 2x² dx + ∫ 3x dx + ∫ 1 dx
- Apply rules:
  - ∫ 2x² dx = 2·(x³/3) = 2x³/3
  - ∫ 3x dx = 3·(x²/2) = 3x²/2
  - ∫ 1 dx = x
- Combine: (2x³/3) + (3x²/2) + x + C

**AI Connection**: Complex loss functions are sums of multiple terms. This rule lets us integrate each term separately.

---

### Example 4: Definite Integral

**Question**: What is ∫[0 to 2] x² dx?

**Solution**:
- Find antiderivative: x³/3
- Evaluate at bounds:
  - At x = 2: (2)³/3 = 8/3
  - At x = 0: (0)³/3 = 0
- Definite integral = 8/3 - 0 = 8/3

**AI Connection**: When calculating probabilities or expected values, we use definite integrals with specific bounds (like 0 to 1 for probabilities).

---

### Example 5: Probability Application

**Question**: A probability density is f(x) = 3x² on [0, 1]. Verify it's valid and find P(0 ≤ X ≤ 0.5).

**Solution**:
- Check total probability: ∫[0 to 1] 3x² dx = 3·(x³/3)|₀¹ = 1³ - 0³ = 1 ✓
- Find P(0 ≤ X ≤ 0.5): ∫[0 to 0.5] 3x² dx = 3·(x³/3)|₀⁰·⁵ = (0.5)³ = 0.125

**AI Connection**: This is exactly how we calculate probabilities for continuous random variables in machine learning models.

---

## 4. Summary / Key Takeaways

- ✅ **Power Rule**: ∫ xⁿ dx = xⁿ⁺¹/(n+1) + C
- ✅ **Constant Multiple**: ∫ c·f(x) dx = c·∫ f(x) dx
- ✅ **Sum Rule**: ∫ [f(x) + g(x)] dx = ∫ f(x) dx + ∫ g(x) dx
- ✅ **Constant of Integration**: Always add +C for indefinite integrals
- ✅ **Definite Integrals**: Evaluate antiderivative at bounds and subtract
- ✅ These rules are essential for probability calculations and optimization in AI

