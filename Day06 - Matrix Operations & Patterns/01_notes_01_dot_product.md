# Day 6 — Dot Product

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Dot Product | Learn how to calculate dot product of vectors |
| 2 | Geometric Interpretation | See dot product as projection and similarity measure |
| 3 | Connect to AI | Understand how dot products measure similarity in embeddings |

---

## 1. Introduction

### What is Dot Product?

The **dot product** (also called inner product) of two vectors is a single number that measures:
- **Similarity**: How aligned the vectors are
- **Projection**: How much one vector projects onto another
- **Angle**: Related to the angle between vectors

### Why Dot Product Matters for AI

Dot products are everywhere in AI:

- **Similarity**: Measure how similar two embeddings are
- **Attention Mechanisms**: Calculate attention weights
- **Neural Networks**: Matrix multiplication uses dot products
- **Recommendation Systems**: Find similar items/users

### Real-World Analogy

Think of dot product like a compatibility score:
- **High dot product**: Vectors point in similar directions (compatible)
- **Low/negative dot product**: Vectors point in different directions (incompatible)
- **Zero dot product**: Vectors are perpendicular (orthogonal)

---

## 2. Deep-Dive Explanation

### Calculation

For vectors u = [u₁, u₂, ..., uₙ] and v = [v₁, v₂, ..., vₙ]:

**Dot Product**: u · v = u₁v₁ + u₂v₂ + ... + uₙvₙ

Multiply corresponding components and sum.

### Geometric Meaning

u · v = ||u|| × ||v|| × cos(θ)

Where:
- ||u|| = magnitude (length) of u
- θ = angle between vectors

**Key Insights**:
- **Same direction**: cos(0°) = 1 → maximum dot product
- **Perpendicular**: cos(90°) = 0 → dot product = 0
- **Opposite direction**: cos(180°) = -1 → minimum (negative) dot product

---

## 3. Instructor Examples

### Example 1: Basic Calculation

**Question**: Calculate [1, 2] · [3, 4].

**Solution**:
- [1, 2] · [3, 4] = 1×3 + 2×4 = 3 + 8 = 11

**AI Connection**: In neural networks, this is exactly what happens in matrix multiplication: each output element is a dot product of a weight row and input vector.

---

### Example 2: Similarity Measure

**Question**: Compare similarity of [1, 1] with [1, 1] vs [1, -1].

**Solution**:
- [1, 1] · [1, 1] = 1 + 1 = 2 (high similarity, same direction)
- [1, 1] · [1, -1] = 1 - 1 = 0 (orthogonal, no similarity)

**AI Connection**: In word embeddings, similar words have high dot products. "king" and "queen" embeddings would have a high dot product.

---

### Example 3: Perpendicular Vectors

**Question**: Find a vector perpendicular to [1, 2].

**Solution**:
- Need u · [1, 2] = 0
- Try [2, -1]: 2×1 + (-1)×2 = 2 - 2 = 0 ✓
- [2, -1] is perpendicular to [1, 2]

**AI Connection**: In some AI applications, we want features to be orthogonal (uncorrelated) to reduce redundancy.

---

### Example 4: Attention Mechanism

**Question**: In attention, we calculate attention weights using dot products. Query q = [1, 2], Key k = [2, 1]. Calculate attention score.

**Solution**:
- Attention score = q · k = [1, 2] · [2, 1] = 2 + 2 = 4
- Higher score = more attention

**AI Connection**: Transformer models use dot products to determine which parts of input to focus on (attention mechanism).

---

## 4. Summary / Key Takeaways

- ✅ **Dot product**: u · v = u₁v₁ + u₂v₂ + ... + uₙvₙ
- ✅ **Geometric meaning**: Measures alignment and angle between vectors
- ✅ **Similarity**: High dot product = similar direction = high similarity
- ✅ **AI applications**: Embeddings, attention, matrix multiplication
- ✅ Dot product is the fundamental similarity measure in vector spaces

