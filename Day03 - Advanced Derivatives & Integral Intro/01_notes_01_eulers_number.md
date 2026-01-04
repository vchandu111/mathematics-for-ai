# Day 3 — Euler's Number

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand e | Learn what Euler's number (e) is and why it's special |
| 2 | Understand eˣ | Learn about the exponential function and its unique property |
| 3 | Connect to AI | See how e is used in activation functions and neural networks |

---

## 1. Introduction

### What is Euler's Number (e)?

**e** is a special mathematical constant approximately equal to **2.71828...**

It's special because:
- eˣ is the only function whose derivative equals itself: d/dx(eˣ) = eˣ
- It appears naturally in growth and decay problems
- It's the base of natural logarithms

### Why e Matters for AI

Euler's number is everywhere in AI:

- **Sigmoid Function**: σ(x) = 1/(1 + e⁻ˣ) - used in neural networks
- **Softmax Function**: Uses eˣ for multi-class classification
- **Activation Functions**: Many neural network activations use e
- **Natural Logarithms**: Used in loss functions and probability calculations

### Real-World Analogy

Think of e like π (pi):
- π appears naturally in circles
- e appears naturally in growth/decay
- Both are fundamental constants that show up everywhere in math and science

In AI: Just like π is fundamental to geometry, e is fundamental to exponential growth and probability.

---

## 2. Deep-Dive Explanation

### The Special Property of eˣ

The function f(x) = eˣ has a unique property:
```
d/dx(eˣ) = eˣ
```

**Meaning**: The derivative of eˣ is eˣ itself! No other function has this property.

### Why This Matters

This makes eˣ perfect for modeling:
- **Exponential Growth**: Populations, investments, viral spread
- **Exponential Decay**: Radioactive decay, cooling, signal attenuation
- **Continuous Compounding**: Interest that compounds continuously

### Visual Representation

```
Graph of eˣ:
        ╱
       ╱
      ╱
     ╱
    ╱
   ╱
  ╱
 ╱

Key points:
- e⁰ = 1
- e¹ = e ≈ 2.718
- As x → ∞, eˣ → ∞ (grows very fast)
- As x → -∞, eˣ → 0 (approaches zero)
```

### Common Values

- e⁰ = 1
- e¹ = e ≈ 2.718
- e² ≈ 7.389
- e⁻¹ = 1/e ≈ 0.368
- e⁻² ≈ 0.135

---

## 3. Instructor Examples

### Example 1: Understanding eˣ

**Question**: What is e⁰ and e¹?

**Solution**:
- e⁰ = 1 (any number to the power of 0 is 1)
- e¹ = e ≈ 2.718

**AI Connection**: In neural networks, we often use e⁰ = 1 as a reference point. The sigmoid function at x = 0 gives 0.5, which is a neutral starting point.

---

### Example 2: Exponential Growth

**Question**: If a quantity grows as f(t) = eᵗ, what is its rate of change?

**Solution**:
- The derivative of eᵗ is eᵗ itself
- This means: the rate of growth equals the current value
- The bigger it gets, the faster it grows!

**AI Connection**: In neural networks, exponential functions can cause values to grow very quickly. This is why we need activation functions like sigmoid that "squash" values between 0 and 1.

---

### Example 3: The Sigmoid Function

**Question**: The sigmoid function is σ(x) = 1/(1 + e⁻ˣ). What happens as x gets very large or very small?

**Solution**:
- As x → +∞: e⁻ˣ → 0, so σ(x) → 1/(1 + 0) = 1
- As x → -∞: e⁻ˣ → +∞, so σ(x) → 1/(1 + ∞) ≈ 0
- At x = 0: σ(0) = 1/(1 + 1) = 0.5

**AI Connection**: The sigmoid function is used as an activation function in neural networks because it smoothly maps any input to a value between 0 and 1, which is perfect for probability outputs.

---

### Example 4: Softmax Function

**Question**: In multi-class classification, we use softmax: softmax(xᵢ) = eˣⁱ / Σeˣʲ. Why use eˣ instead of just x?

**Solution**:
- Using eˣ ensures all outputs are positive
- It amplifies differences: larger inputs get much larger outputs
- The sum of all softmax outputs equals 1 (perfect for probabilities)

**AI Connection**: Softmax is the standard output layer for multi-class classification. It converts raw scores into probabilities that sum to 1, making it perfect for "this image is 70% cat, 20% dog, 10% bird" type predictions.

---

## 4. Summary / Key Takeaways

- ✅ **e** ≈ 2.718 is a fundamental constant
- ✅ **eˣ** is unique: its derivative equals itself (d/dx(eˣ) = eˣ)
- ✅ **Sigmoid function** uses e: σ(x) = 1/(1 + e⁻ˣ) - maps to [0, 1]
- ✅ **Softmax function** uses eˣ for multi-class probability outputs
- ✅ e appears naturally in exponential growth, decay, and probability
- ✅ Understanding e helps understand activation functions in neural networks

