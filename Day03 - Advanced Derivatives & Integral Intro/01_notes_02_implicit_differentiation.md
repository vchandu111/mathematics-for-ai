# Day 3 — Implicit Differentiation

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Implicit Functions | Learn when functions aren't explicitly solved for y |
| 2 | Apply Chain Rule | Use chain rule to differentiate implicitly |
| 3 | Connect to AI | See how implicit differentiation appears in backpropagation |

---

## 1. Introduction

### What is Implicit Differentiation?

Usually, we see functions like y = x² (explicit form). But sometimes we have equations like x² + y² = 25 where y isn't isolated.

**Implicit differentiation** lets us find dy/dx even when y isn't explicitly written as a function of x.

### Why Implicit Differentiation Matters for AI

In AI, we often deal with:

- **Complex relationships**: Variables that depend on each other in non-obvious ways
- **Backpropagation**: Calculating gradients through layers where variables are implicitly related
- **Optimization constraints**: When variables must satisfy certain relationships

### Real-World Analogy

Think of it like a recipe:
- **Explicit**: "Add 2 cups of flour" (clear instruction)
- **Implicit**: "The total should be 5 cups" (relationship, but not explicit amounts)

In AI: We know the relationship between variables (like error depends on weights), but we need to find how changing one affects the other.

---

## 2. Deep-Dive Explanation

### The Key Idea

When we differentiate both sides of an equation with respect to x, we treat y as a function of x (even if we don't know what that function is).

**Important**: When differentiating terms with y, we use the **chain rule**:
- d/dx(y²) = 2y · dy/dx
- d/dx(y³) = 3y² · dy/dx
- d/dx(xy) = x·dy/dx + y·dx/dx = x·dy/dx + y

### Step-by-Step Process

1. Differentiate both sides with respect to x
2. Apply chain rule to y terms (multiply by dy/dx)
3. Collect all dy/dx terms on one side
4. Solve for dy/dx

### Visual Example

```
Equation: x² + y² = 25

Differentiate both sides:
d/dx(x²) + d/dx(y²) = d/dx(25)
2x + 2y·dy/dx = 0

Solve for dy/dx:
2y·dy/dx = -2x
dy/dx = -x/y
```

---

## 3. Instructor Examples

### Example 1: Circle Equation

**Question**: Find dy/dx for x² + y² = 25.

**Solution**:
- Differentiate both sides: d/dx(x²) + d/dx(y²) = d/dx(25)
- 2x + 2y·dy/dx = 0
- Solve: 2y·dy/dx = -2x
- dy/dx = -x/y

**AI Connection**: In optimization, we often have constraint equations. Implicit differentiation helps us understand how variables relate under constraints.

---

### Example 2: Product with y

**Question**: Find dy/dx for xy = 10.

**Solution**:
- Differentiate: d/dx(xy) = d/dx(10)
- Use product rule: x·dy/dx + y·1 = 0
- Solve: x·dy/dx = -y
- dy/dx = -y/x

**AI Connection**: In neural networks, we have products like (weight × input). Understanding how these relate helps with gradient calculations.

---

### Example 3: More Complex

**Question**: Find dy/dx for x²y + y² = 5.

**Solution**:
- Differentiate: d/dx(x²y) + d/dx(y²) = d/dx(5)
- For x²y, use product rule: (2x)·y + x²·dy/dx
- For y²: 2y·dy/dx
- Combine: 2xy + x²·dy/dx + 2y·dy/dx = 0
- Factor dy/dx: x²·dy/dx + 2y·dy/dx = -2xy
- dy/dx(x² + 2y) = -2xy
- dy/dx = -2xy / (x² + 2y)

**AI Connection**: Complex loss functions in deep learning have multiple terms. Implicit differentiation helps us understand how all the pieces relate.

---

### Example 4: Exponential with y

**Question**: Find dy/dx for eʸ = x.

**Solution**:
- Differentiate: d/dx(eʸ) = d/dx(x)
- Chain rule: eʸ·dy/dx = 1
- Solve: dy/dx = 1/eʸ = 1/x (since eʸ = x)

**AI Connection**: Activation functions like sigmoid use exponentials. Understanding their derivatives is crucial for backpropagation.

---

## 4. Summary / Key Takeaways

- ✅ **Implicit differentiation** finds dy/dx when y isn't explicitly solved
- ✅ **Chain rule** is key: d/dx(yⁿ) = n·yⁿ⁻¹·dy/dx
- ✅ **Process**: Differentiate both sides, collect dy/dx terms, solve for dy/dx
- ✅ Used in AI for complex relationships in backpropagation and constrained optimization
- ✅ Helps understand how variables relate when they're not in explicit form

