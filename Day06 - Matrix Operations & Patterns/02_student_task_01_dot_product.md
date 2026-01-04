# Day 6 — Student Task: Dot Product

## Instructions

Calculate dot products and understand their geometric and AI meanings. Show your calculations clearly.

---

## Tasks

### Task 1: Basic Dot Products (Easy)

Calculate:
- a) [1, 2] · [3, 4]
- b) [2, -1] · [3, 2]
- c) [1, 1, 1] · [2, 3, 4]
- d) [0, 0] · [5, 6]

**Expected Output**: Four dot product values with work shown.

---

### Task 2: Similarity Analysis (Easy)

Compare dot products to assess similarity:
- a) [1, 0] · [1, 0] (same vector)
- b) [1, 0] · [0, 1] (perpendicular)
- c) [1, 0] · [-1, 0] (opposite)
- d) [1, 1] · [2, 2] (scaled version)

**Expected Output**: Four dot product values with brief interpretation of similarity.

---

### Task 3: Medium Reasoning Question

For vectors u = [3, 4] and v = [1, 2]:

- a) Calculate u · v
- b) Calculate v · u
- c) Are they equal? What property does this demonstrate?
- d) Calculate (2u) · v and 2(u · v). Are they equal?

**Expected Output**: 
- Two dot product values
- Comparison showing commutativity
- Two calculations showing scalar multiplication property

---

### Task 4: Application to AI (Medium)

In word embeddings, word vectors are:
- "cat" = [1, 2, 3]
- "dog" = [2, 3, 4]
- "car" = [-1, -2, -3]

- a) Calculate similarity: "cat" · "dog"
- b) Calculate similarity: "cat" · "car"
- c) Which pair is more similar? Why does this make sense?
- d) What does a negative dot product indicate?

**Expected Output**: 
- Two similarity scores
- Comparison and explanation
- Written interpretation

---

### Task 5: Perpendicular Vectors (Medium)

Find a vector perpendicular to:
- a) [1, 2] (hint: need dot product = 0)
- b) [3, 1]
- c) [2, -3]

**Expected Output**: Three perpendicular vectors with verification (dot product = 0).

---

### Task 6: Medium Reasoning Question

In a neural network, a weight vector w = [0.5, 0.3, 0.2] computes output as w · x.

- a) If input x = [1, 1, 1], what is the output?
- b) If input x = [2, 0, 0], what is the output?
- c) Which input produces a larger output? Why?
- d) What does this tell us about how the neuron responds to different inputs?

**Expected Output**: 
- Two output values
- Comparison
- Written explanation

---

### Task 7: Optional Python Task

Write Python code to calculate dot products:

```python
import numpy as np

def dot_product(u, v):
    # Calculate dot product
    return result
```

Test with examples from Task 1.

**Expected Output**: Python code with function and test cases.

---

## Expected Output / Answer Format

For each task, provide:
- **Dot product values**: Numeric results
- **Work shown**: Step-by-step calculations
- **Interpretations**: Brief explanations of what values mean
- **Verifications**: Check perpendicular vectors have dot product = 0

**Note**: No solutions are provided—work through each problem independently!

