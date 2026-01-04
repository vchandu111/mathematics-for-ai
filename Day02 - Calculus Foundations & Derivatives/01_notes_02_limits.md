# Day 2 — Limits

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Limits Conceptually | Learn what limits mean: approaching a value |
| 2 | Calculate Simple Limits | Master basic limit calculations |
| 3 | Connect Limits to Derivatives | See how limits are the foundation of derivatives |

---

## 1. Introduction

### What is a Limit?

A **limit** answers the question: "What value does a function approach as the input gets closer and closer to a certain point?"

Think of it like this: You're walking toward a wall. You can get closer and closer, but you might never actually touch it. The limit tells us what value you're approaching.

### Why Limits Matter for AI

Limits are the mathematical foundation for derivatives, which are essential for:

- **Gradient Calculation**: Derivatives (used in backpropagation) are defined using limits
- **Optimization**: Finding optimal points requires understanding how functions behave near certain values
- **Numerical Stability**: Understanding limits helps prevent division by zero and other numerical issues in AI

### Real-World Analogy

Imagine zooming in on a curve with a microscope:
- As you zoom in more and more, the curve looks more and more like a straight line
- The limit tells us what that straight line's slope is
- This is exactly how we calculate derivatives!

---

## 2. Deep-Dive Explanation

### The Limit Notation

```
lim f(x) = L
x→a
```

This reads: "The limit of f(x) as x approaches a equals L"

**Meaning**: As x gets closer and closer to a, f(x) gets closer and closer to L.

### Key Insight: Approaching, Not Reaching

The limit is about what value we're **approaching**, not necessarily what the function equals at that point.

**Example**:
- Function: f(x) = (x² - 1) / (x - 1)
- At x = 1, the function is undefined (0/0)
- But as x approaches 1, the function approaches 2
- So: lim(x→1) f(x) = 2

### Visual Representation

```
Function approaching a limit:
         ●
        / \
       /   \
      /     \
     /       \
    /         \
   /           \
  /             \
 /               \
/                 \

As we zoom in near the point, the function approaches a specific value
```

### Simple Limit Rules

1. **Direct Substitution**: If f(a) exists, then lim(x→a) f(x) = f(a)
2. **Constant**: lim(x→a) c = c (constant stays constant)
3. **Linear**: lim(x→a) x = a

---

## 3. Instructor Examples

### Example 1: Simple Limit

**Question**: What is lim(x→3) (2x + 1)?

**Solution**:
- As x approaches 3, we can substitute x = 3
- f(3) = 2(3) + 1 = 6 + 1 = 7
- So: lim(x→3) (2x + 1) = 7

**AI Connection**: This is like evaluating a function at a point. In AI, we often need to know function values at specific inputs.

---

### Example 2: Limit That Requires Simplification

**Question**: What is lim(x→2) (x² - 4) / (x - 2)?

**Solution**:
- Direct substitution gives 0/0 (undefined)
- Factor the numerator: x² - 4 = (x - 2)(x + 2)
- Simplify: (x² - 4)/(x - 2) = (x - 2)(x + 2)/(x - 2) = x + 2
- Now: lim(x→2) (x + 2) = 2 + 2 = 4

**AI Connection**: Sometimes AI calculations hit undefined forms. Understanding limits helps us handle these cases properly.

---

### Example 3: Approaching from Different Sides

**Question**: Consider f(x) = 1/x. What happens as x approaches 0?

**Solution**:
- As x approaches 0 from the right (positive side): 1/x → +∞
- As x approaches 0 from the left (negative side): 1/x → -∞
- The limit doesn't exist because it approaches different values from different sides

**AI Connection**: In gradient descent, we need to be careful about functions that behave differently in different directions. This affects optimization.

---

### Example 4: Limit and Derivatives Connection

**Question**: The derivative is defined as a limit. If we want the derivative of f(x) = x² at x = 2, we calculate:

lim(h→0) [f(2+h) - f(2)] / h

What does this represent?

**Solution**:
- f(2+h) = (2+h)² = 4 + 4h + h²
- f(2) = 4
- [f(2+h) - f(2)] / h = (4h + h²) / h = 4 + h
- lim(h→0) (4 + h) = 4

**AI Connection**: This is exactly how we calculate gradients in neural networks! The limit gives us the instantaneous rate of change, which is what we need for backpropagation.

---

## 4. Summary / Key Takeaways

- ✅ **Limit** = the value a function approaches as input approaches a point
- ✅ Limits can exist even when the function is undefined at that point
- ✅ Limits are the foundation of derivatives (derivatives are defined using limits)
- ✅ Understanding limits helps with numerical stability in AI calculations
- ✅ The notation lim(x→a) f(x) means "limit of f(x) as x approaches a"

