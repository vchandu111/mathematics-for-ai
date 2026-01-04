# Day 6 — Cross Product

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Cross Product | Learn cross product in 3D (vector perpendicular to two vectors) |
| 2 | Calculate Cross Products | Master the cross product formula |
| 3 | Connect to AI | See how cross products appear in some ML applications |

---

## 1. Introduction

### What is Cross Product?

The **cross product** of two 3D vectors produces a third vector that is:
- **Perpendicular** to both input vectors
- **Magnitude** = area of parallelogram formed by inputs
- **Direction** given by right-hand rule

### Why Cross Product Matters

- **Normal Vectors**: Find perpendicular directions (useful in graphics, some ML)
- **Area/Volume**: Calculate areas and volumes
- **Orientation**: Determine orientation in 3D space

---

## 2. Deep-Dive Explanation

### Formula

For u = [u₁, u₂, u₃] and v = [v₁, v₂, v₃]:

**u × v = [u₂v₃ - u₃v₂, u₃v₁ - u₁v₃, u₁v₂ - u₂v₁]**

### Properties

- **u × v = -(v × u)**: Anti-commutative
- **u × u = 0**: Cross product with itself is zero vector
- **Perpendicular**: Result is perpendicular to both u and v

---

## 3. Instructor Examples

### Example 1: Basic Cross Product

**Question**: Calculate [1, 0, 0] × [0, 1, 0].

**Solution**:
- [1, 0, 0] × [0, 1, 0] = [0×0 - 0×1, 0×0 - 1×0, 1×1 - 0×0] = [0, 0, 1]
- Result is [0, 0, 1] (z-axis unit vector)

**AI Connection**: Cross products help find orthogonal directions, useful in some dimensionality reduction techniques.

---

### Example 2: Perpendicular Vector

**Question**: Find a vector perpendicular to both [1, 1, 0] and [1, 0, 1].

**Solution**:
- Cross product gives perpendicular vector
- [1, 1, 0] × [1, 0, 1] = [1×1 - 0×0, 0×1 - 1×1, 1×0 - 1×1] = [1, -1, -1]

**AI Connection**: Finding orthogonal directions is important in feature engineering and some ML algorithms.

---

## 4. Summary / Key Takeaways

- ✅ **Cross product**: Produces vector perpendicular to two input vectors
- ✅ **Formula**: u × v = [u₂v₃ - u₃v₂, u₃v₁ - u₁v₃, u₁v₂ - u₂v₁]
- ✅ **Anti-commutative**: u × v = -(v × u)
- ✅ **AI Connection**: Used for finding orthogonal directions and normal vectors
- ✅ Less common than dot product in AI, but appears in specialized applications

