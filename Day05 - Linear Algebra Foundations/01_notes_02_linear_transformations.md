# Day 5 — Linear Transformations

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Transformations | Learn how matrices transform vectors |
| 2 | Visualize Transformations | See rotations, scaling, and shearing |
| 3 | Connect to Neural Networks | Understand how layers transform data |

---

## 1. Introduction

### What are Linear Transformations?

A **linear transformation** takes a vector and produces another vector. It's like a function for vectors:
- Input: vector v
- Output: transformed vector T(v)

**Key Property**: T(a·u + b·v) = a·T(u) + b·T(v) (preserves addition and scaling)

### Why Transformations Matter for AI

Every layer in a neural network is a linear transformation:

- **Input Layer**: Transforms raw data
- **Hidden Layers**: Each applies a transformation (matrix multiplication)
- **Output Layer**: Final transformation to predictions

### Real-World Analogy

Think of transformations like filters or effects:
- **Rotation**: Turn the vector
- **Scaling**: Stretch or shrink
- **Reflection**: Flip the vector
- **Neural Network Layer**: All of these combined!

---

## 2. Deep-Dive Explanation

### Common Transformations

**Scaling**: Multiply each component
- [2, 0; 0, 2] scales by 2 in both directions

**Rotation**: Rotate around origin
- Rotates vectors by an angle

**Reflection**: Flip across a line
- Mirrors vectors

### Matrix Representation

Every linear transformation can be represented by a matrix:
- T(v) = A·v (matrix A times vector v)

### Visual Examples

```
Scaling:
[2, 0]   [1]   [2]
[0, 2] × [1] = [2]  (doubles the vector)

Rotation (90°):
[0, -1]   [1]   [0]
[1,  0] × [0] = [1]  (rotates 90°)
```

---

## 3. Instructor Examples

### Example 1: Scaling Transformation

**Question**: What does the matrix [3, 0; 0, 3] do to vector [1, 2]?

**Solution**:
- [3, 0; 0, 3] × [1, 2] = [3×1 + 0×2, 0×1 + 3×2] = [3, 6]
- Scales the vector by 3 in all directions

**AI Connection**: In neural networks, weights scale input features. This is exactly what happens in each layer.

---

### Example 2: Rotation

**Question**: Rotate vector [1, 0] by 90° counterclockwise.

**Solution**:
- Rotation matrix: [0, -1; 1, 0]
- [0, -1; 1, 0] × [1, 0] = [0, 1]
- The vector [1, 0] (pointing right) becomes [0, 1] (pointing up)

**AI Connection**: Transformations in neural networks can rotate and reorient feature spaces to better separate classes.

---

### Example 3: Combined Transformations

**Question**: Apply scaling then rotation. What's the combined effect?

**Solution**:
- First scale: [2, 0; 0, 2] × [1, 1] = [2, 2]
- Then rotate: [0, -1; 1, 0] × [2, 2] = [-2, 2]
- Combined: multiple transformations = multiple matrix multiplications

**AI Connection**: Deep neural networks apply many transformations in sequence. Each layer transforms the output of the previous layer.

---

## 4. Summary / Key Takeaways

- ✅ **Linear transformation** = function that maps vectors to vectors
- ✅ **Matrix representation**: T(v) = A·v
- ✅ **Common types**: Scaling, rotation, reflection, shearing
- ✅ **Neural networks**: Each layer is a linear transformation (followed by activation)
- ✅ Transformations are the core operations in all neural network layers

