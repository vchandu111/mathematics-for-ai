# Day 4 — Indefinite Integrals

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Master Indefinite Integrals | Learn to find antiderivatives with the constant of integration |
| 2 | Apply Integration Rules | Use power rule, constant multiple, and sum rules for integration |
| 3 | Connect to AI Functions | See how indefinite integrals help understand AI model functions |

---

## 1. Introduction

### What are Indefinite Integrals?

An **indefinite integral** is the general antiderivative of a function. It includes the constant of integration (+C) because the derivative of any constant is zero.

**Notation**: ∫ f(x) dx = F(x) + C

This means: "Find all functions whose derivative is f(x)"

### Why Indefinite Integrals Matter for AI

Indefinite integrals help us:

- **Understand Functions**: Work backwards from derivatives to original functions
- **Model Building**: Construct functions that satisfy certain derivative properties
- **General Solutions**: Find families of functions that work for optimization problems
- **Theoretical Understanding**: Deepen understanding of how functions relate to their rates of change

### Real-World Analogy

Think of indefinite integrals like "reverse engineering":
- **Derivative**: "I have a car's speed over time, what's the position?" (breaking down)
- **Indefinite Integral**: "I know how speed changes, find all possible position functions" (building up)

In AI: We often know how error changes (derivative), and indefinite integrals help us understand the possible error functions.

---

## 2. Deep-Dive Explanation

### The Constant of Integration

When we integrate, we add +C because:
- If F(x) is an antiderivative, then F(x) + 5 is also an antiderivative
- If F(x) is an antiderivative, then F(x) - 100 is also an antiderivative
- All differ by a constant, and the derivative of any constant is 0

**Example**:
- ∫ 2x dx = x² + C
- Both x² + 5 and x² - 3 are valid antiderivatives (their derivatives both equal 2x)

### Integration Rules Recap

1. **Power Rule**: ∫ xⁿ dx = xⁿ⁺¹/(n+1) + C (n ≠ -1)
2. **Constant Multiple**: ∫ c·f(x) dx = c·∫ f(x) dx
3. **Sum Rule**: ∫ [f(x) + g(x)] dx = ∫ f(x) dx + ∫ g(x) dx

### Key Difference: Indefinite vs Definite

- **Indefinite**: ∫ f(x) dx = F(x) + C (general solution, includes +C)
- **Definite**: ∫[a to b] f(x) dx = F(b) - F(a) (specific number, no +C needed)

---

## 3. Instructor Examples

### Example 1: Simple Power Rule

**Question**: Find ∫ x³ dx.

**Solution**:
- Using power rule: ∫ x³ dx = x³⁺¹/(3+1) + C = x⁴/4 + C

**AI Connection**: Many loss functions in AI are polynomials. Knowing their antiderivatives helps understand the total error landscape.

---

### Example 2: Constant Multiple

**Question**: Find ∫ 5x² dx.

**Solution**:
- Factor constant: 5·∫ x² dx
- Apply power rule: 5·(x³/3) + C = (5x³/3) + C

**AI Connection**: In neural networks, weights are often multiplied by constants. This rule helps integrate such terms.

---

### Example 3: Sum of Terms

**Question**: Find ∫ (3x² + 2x + 1) dx.

**Solution**:
- Split: ∫ 3x² dx + ∫ 2x dx + ∫ 1 dx
- Apply rules:
  - ∫ 3x² dx = 3·(x³/3) = x³
  - ∫ 2x dx = 2·(x²/2) = x²
  - ∫ 1 dx = x
- Combine: x³ + x² + x + C

**AI Connection**: Loss functions are often sums of multiple terms (like mean squared error). This rule lets us integrate each term separately.

---

### Example 4: Verifying the Answer

**Question**: Verify that ∫ 4x³ dx = x⁴ + C is correct.

**Solution**:
- Take derivative of x⁴ + C: d/dx(x⁴ + C) = 4x³ ✓
- This confirms our antiderivative is correct!

**AI Connection**: Always verify integration results in AI applications. A small error in integration can lead to wrong optimization results.

---

### Example 5: Understanding the Constant

**Question**: Why do we need +C in ∫ 2x dx = x² + C?

**Solution**:
- If we only wrote x², we'd be missing other valid antiderivatives
- x² + 5, x² - 10, x² + π are all valid antiderivatives of 2x
- The +C represents all possible constants
- When we have initial conditions, we can solve for C

**AI Connection**: In optimization, the constant C might represent a baseline error level. Different models might have different baselines, but the same rate of change.

---

## 4. Summary / Key Takeaways

- ✅ **Indefinite integral** = general antiderivative with +C
- ✅ **Power Rule**: ∫ xⁿ dx = xⁿ⁺¹/(n+1) + C
- ✅ **Constant Multiple**: ∫ c·f(x) dx = c·∫ f(x) dx
- ✅ **Sum Rule**: ∫ [f(x) + g(x)] dx = ∫ f(x) dx + ∫ g(x) dx
- ✅ Always include +C for indefinite integrals
- ✅ Verify answers by taking derivatives
- ✅ Used in AI to understand function families and model structures

