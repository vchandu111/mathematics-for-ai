# Day 1 — Combinatorics

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Permutations | Learn how to count arrangements where order matters |
| 2 | Understand Combinations | Learn how to count selections where order doesn't matter |
| 3 | Apply Combinatorics to AI | See how counting methods are used in AI algorithms and data analysis |

---

## 1. Introduction

### What is Combinatorics?

Combinatorics is the branch of mathematics that deals with counting. It helps us answer questions like:
- "How many ways can I arrange these items?"
- "How many ways can I choose a subset from a larger set?"

### Why Combinatorics Matters for AI

Combinatorics is essential in AI for:

- **Feature Selection**: "How many ways can we choose 5 features from 20 available features?"
- **Neural Network Architecture**: "How many different network configurations are possible?"
- **Search Algorithms**: "How many paths exist in a decision tree?"
- **Data Sampling**: "How many ways can we split a dataset into training and testing sets?"
- **Password/Key Generation**: "How many possible passwords can be created?"

### Real-World Analogy

Think of combinatorics like a combination lock:
- **Permutation** (order matters): 1234 is different from 4321
- **Combination** (order doesn't matter): Choosing {apple, banana} is the same as {banana, apple}

---

## 2. Deep-Dive Explanation

### Permutations (Order Matters)

**Permutation** = Arrangements where the order is important.

**Formula**: 
```
P(n, r) = n! / (n - r)!
```

Where:
- `n` = total items
- `r` = items we're arranging
- `!` = factorial (e.g., 5! = 5 × 4 × 3 × 2 × 1 = 120)

**Example**: How many ways can we arrange 3 books from a shelf of 5?
- P(5, 3) = 5! / (5-3)! = 5! / 2! = (5×4×3×2×1) / (2×1) = 60 ways

### Combinations (Order Doesn't Matter)

**Combination** = Selections where the order is NOT important.

**Formula**:
```
C(n, r) = n! / [r! × (n - r)!]
```

Also written as: C(n, r) = nCr = (n choose r)

**Example**: How many ways can we choose 3 books from a shelf of 5 (order doesn't matter)?
- C(5, 3) = 5! / [3! × (5-3)!] = 5! / (3! × 2!) = 120 / (6 × 2) = 10 ways

### Visual Comparison

```
PERMUTATIONS (Order Matters):
Books: A, B, C
Arrangements: ABC, ACB, BAC, BCA, CAB, CBA = 6 ways

COMBINATIONS (Order Doesn't Matter):
Books: A, B, C
Selections: {A, B, C} = 1 way (ABC, ACB, BAC, etc. are all the same)
```

### Factorials Quick Reference

```
0! = 1
1! = 1
2! = 2 × 1 = 2
3! = 3 × 2 × 1 = 6
4! = 4 × 3 × 2 × 1 = 24
5! = 5 × 4 × 3 × 2 × 1 = 120
```

---

## 3. Instructor Examples

### Example 1: Password Combinations

**Question**: How many 4-digit PIN codes can be created using digits 0-9 (digits can repeat)?

**Solution**:
- Each position can be any digit (0-9) = 10 choices
- Total positions = 4
- Total combinations = 10 × 10 × 10 × 10 = 10⁴ = 10,000

**AI Connection**: This is why longer passwords are more secure—more combinations mean harder to crack. AI security systems use combinatorics to assess password strength.

---

### Example 2: Feature Selection

**Question**: An AI model has 10 features available. How many ways can we choose 3 features to use?

**Solution**:
- Order doesn't matter (choosing features A, B, C is the same as C, B, A)
- This is a **combination**: C(10, 3)
- C(10, 3) = 10! / [3! × (10-3)!] = 10! / (3! × 7!)
- = (10 × 9 × 8) / (3 × 2 × 1) = 720 / 6 = 120 ways

**AI Connection**: Feature selection is crucial in machine learning. With 10 features, there are 120 different ways to choose 3, and each combination might perform differently!

---

### Example 3: Arranging Data Points

**Question**: How many ways can we arrange 5 different data points in a sequence?

**Solution**:
- Order matters (arrangement A-B-C-D-E is different from E-D-C-B-A)
- This is a **permutation**: P(5, 5) = 5!
- 5! = 5 × 4 × 3 × 2 × 1 = 120 ways

**AI Connection**: When training neural networks, the order of training data can matter. Combinatorics helps us understand how many different training sequences are possible.

---

### Example 4: Committee Selection

**Question**: From a team of 8 data scientists, how many ways can we form a committee of 4?

**Solution**:
- Order doesn't matter (committee {Alice, Bob, Charlie, Diana} is the same regardless of order)
- This is a **combination**: C(8, 4)
- C(8, 4) = 8! / [4! × (8-4)!] = 8! / (4! × 4!)
- = (8 × 7 × 6 × 5) / (4 × 3 × 2 × 1) = 1680 / 24 = 70 ways

**AI Connection**: In ensemble learning, we might want to combine predictions from different subsets of models. Combinatorics tells us how many different model combinations are possible.

---

## 4. Summary / Key Takeaways

- ✅ **Permutations** count arrangements where **order matters**: P(n, r) = n! / (n - r)!
- ✅ **Combinations** count selections where **order doesn't matter**: C(n, r) = n! / [r! × (n - r)!]
- ✅ **Factorial** (n!) = product of all positive integers up to n
- ✅ Combinatorics is used in AI for feature selection, model architecture design, and search algorithms
- ✅ When order matters → use Permutation; when order doesn't matter → use Combination

