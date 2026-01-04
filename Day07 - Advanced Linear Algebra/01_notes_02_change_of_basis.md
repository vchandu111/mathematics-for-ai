# Day 7 — Change of Basis

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Basis | Learn what a basis is (set of independent vectors) |
| 2 | Change Coordinates | See how to represent vectors in different bases |
| 3 | Connect to AI | Understand how PCA and dimensionality reduction work |

---

## 1. Introduction

### What is Change of Basis?

A **basis** is a set of independent vectors that span a space. We can represent the same vector in different bases (coordinate systems).

**Change of basis** = converting coordinates from one basis to another.

### Why Change of Basis Matters for AI

- **PCA**: Principal Component Analysis finds a new basis (principal components)
- **Dimensionality Reduction**: Project data onto lower-dimensional basis
- **Feature Transformation**: Transform features to better basis for learning

---

## 2. Deep-Dive Explanation

### Standard Basis

In 2D, standard basis is:
- e₁ = [1, 0]
- e₂ = [0, 1]

Any vector [a, b] = a·e₁ + b·e₂

### New Basis

New basis vectors:
- v₁ = [1, 1]
- v₂ = [-1, 1]

To convert: find coefficients to express vector in new basis.

---

## 3. Instructor Examples

### Example 1: Understanding Basis

**Question**: Do [1, 0] and [0, 1] form a basis for 2D?

**Solution**:
- Yes! They're independent and span 2D space
- Any vector [a, b] = a·[1, 0] + b·[0, 1]

**AI Connection**: Standard basis represents raw features. PCA finds a better basis (principal components) that captures most variance.

---

### Example 2: PCA Intuition

**Question**: Why change basis in PCA?

**Solution**:
- Original basis might have correlated features
- New basis (principal components) has uncorrelated directions
- First component captures most variance
- Allows dimensionality reduction

**AI Connection**: PCA finds basis where first few components contain most information, enabling compression.

---

## 4. Summary / Key Takeaways

- ✅ **Basis**: Set of independent vectors spanning a space
- ✅ **Change of basis**: Convert coordinates between different bases
- ✅ **PCA**: Finds optimal basis (principal components) for data
- ✅ **Dimensionality reduction**: Use fewer basis vectors to represent data
- ✅ Change of basis enables efficient data representation in AI

