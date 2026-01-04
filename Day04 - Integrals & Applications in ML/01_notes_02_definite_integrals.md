# Day 4 — Definite Integrals

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Definite Integrals | Learn that definite integrals calculate specific areas/values |
| 2 | Apply Fundamental Theorem | Use F(b) - F(a) to evaluate definite integrals |
| 3 | Connect to AI Applications | See how definite integrals calculate probabilities and expected values |

---

## 1. Introduction

### What are Definite Integrals?

A **definite integral** calculates the exact area under a curve between two specific points, or the exact accumulated value over a range.

**Notation**: ∫[a to b] f(x) dx

This gives a **specific number** (not a function), representing the area from x = a to x = b.

### Why Definite Integrals Matter for AI

Definite integrals are essential for:

- **Probability Calculations**: Total probability over a range
- **Expected Values**: Average outcomes in continuous distributions
- **Area Under ROC Curves**: Evaluating classifier performance
- **Loss Function Integration**: Calculating total error over ranges

### Real-World Analogy

Think of definite integrals like a bank statement:
- **Indefinite**: "Here's a formula for your balance" (general)
- **Definite**: "Your balance from Jan 1 to Jan 31 is $500" (specific)

In AI: We use definite integrals to get specific probabilities like "P(0.3 ≤ score ≤ 0.7) = 0.4"

---

## 2. Deep-Dive Explanation

### The Fundamental Theorem of Calculus

If F(x) is an antiderivative of f(x), then:
```
∫[a to b] f(x) dx = F(b) - F(a)
```

**Process**:
1. Find antiderivative F(x)
2. Evaluate F(b)
3. Evaluate F(a)
4. Subtract: F(b) - F(a)

### Key Difference from Indefinite

- **Indefinite**: ∫ f(x) dx = F(x) + C (function with +C)
- **Definite**: ∫[a to b] f(x) dx = F(b) - F(a) (specific number, no +C)

The constant C cancels out when we subtract!

### Visual Representation

```
Area under curve from a to b:
     │
     │    ╱───╲
     │   ╱     ╲
     │  ╱       ╲
     │ ╱         ╲
     │╱           ╲
    ─┴─────────────┴─
    a              b

Area = ∫[a to b] f(x) dx = F(b) - F(a)
```

---

## 3. Instructor Examples

### Example 1: Simple Definite Integral

**Question**: Evaluate ∫[0 to 3] x² dx.

**Solution**:
- Antiderivative: F(x) = x³/3
- Evaluate at bounds:
  - F(3) = (3)³/3 = 27/3 = 9
  - F(0) = (0)³/3 = 0
- Definite integral = 9 - 0 = 9

**AI Connection**: This represents the total accumulated value. In probability, this would be the total probability over the range.

---

### Example 2: Probability Calculation

**Question**: A probability density is f(x) = 2x on [0, 1]. Find P(0 ≤ X ≤ 0.5).

**Solution**:
- P(0 ≤ X ≤ 0.5) = ∫[0 to 0.5] 2x dx
- Antiderivative: F(x) = x²
- Evaluate:
  - F(0.5) = (0.5)² = 0.25
  - F(0) = (0)² = 0
- Probability = 0.25 - 0 = 0.25

**AI Connection**: This is exactly how we calculate probabilities for continuous random variables in machine learning models.

---

### Example 3: Area Interpretation

**Question**: What is the area under f(x) = 3x from x = 1 to x = 4?

**Solution**:
- Area = ∫[1 to 4] 3x dx
- Antiderivative: F(x) = (3/2)x²
- Evaluate:
  - F(4) = (3/2)(4)² = (3/2)(16) = 24
  - F(1) = (3/2)(1)² = 3/2 = 1.5
- Area = 24 - 1.5 = 22.5

**AI Connection**: In optimization, we might integrate the rate of improvement to find total improvement over a training period.

---

### Example 4: Verifying Probability Distribution

**Question**: Verify that f(x) = 3x² on [0, 1] is a valid probability density.

**Solution**:
- For a valid PDF, total probability must equal 1
- Total = ∫[0 to 1] 3x² dx
- Antiderivative: F(x) = x³
- Evaluate:
  - F(1) = (1)³ = 1
  - F(0) = (0)³ = 0
- Total = 1 - 0 = 1 ✓ (valid!)

**AI Connection**: All probability density functions must integrate to 1 over their domain. This is a fundamental requirement we check.

---

### Example 5: Expected Value Setup

**Question**: For f(x) = 2x on [0, 1], set up the integral for expected value E[X].

**Solution**:
- Expected value: E[X] = ∫[0 to 1] x·f(x) dx
- = ∫[0 to 1] x·(2x) dx = ∫[0 to 1] 2x² dx
- Antiderivative: F(x) = (2/3)x³
- Evaluate:
  - F(1) = (2/3)(1)³ = 2/3
  - F(0) = (2/3)(0)³ = 0
- E[X] = 2/3 - 0 = 2/3

**AI Connection**: Expected values are crucial in AI for understanding average model performance, average prediction scores, etc.

---

## 4. Summary / Key Takeaways

- ✅ **Definite integral** = specific number (area/accumulated value) from a to b
- ✅ **Fundamental Theorem**: ∫[a to b] f(x) dx = F(b) - F(a)
- ✅ **No +C needed**: The constant cancels out when subtracting
- ✅ Used in AI for: probability calculations, expected values, performance metrics
- ✅ Process: Find antiderivative → Evaluate at bounds → Subtract

