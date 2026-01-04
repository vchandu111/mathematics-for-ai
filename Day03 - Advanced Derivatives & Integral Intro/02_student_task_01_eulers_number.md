# Day 3 — Student Task: Euler's Number

## Instructions

Complete these tasks to understand Euler's number (e) and its applications. You may use a calculator for eˣ values, or approximate e ≈ 2.718. Show your reasoning for each answer.

---

## Tasks

### Task 1: Basic e Values (Easy)

Calculate or identify:
- a) e⁰
- b) e¹
- c) e⁻¹ (1/e)
- d) e² (approximate)

**Expected Output**: Four numeric values (use e ≈ 2.718 for approximations).

---

### Task 2: Understanding eˣ Behavior (Easy)

Consider the function f(x) = eˣ.

Answer:
- a) What is f(0)?
- b) What happens to f(x) as x becomes very large (x → +∞)?
- c) What happens to f(x) as x becomes very negative (x → -∞)?
- d) Is f(x) ever negative? Why or why not?

**Expected Output**: Written explanations for all four parts.

---

### Task 3: Medium Reasoning Question

The sigmoid function is σ(x) = 1/(1 + e⁻ˣ).

Calculate:
- a) σ(0)
- b) σ(1) (approximate, using e ≈ 2.718)
- c) σ(-1) (approximate)
- d) What value does σ(x) approach as x → +∞?
- e) What value does σ(x) approach as x → -∞?

**Expected Output**: Five numeric values with brief explanations.

---

### Task 4: Medium Reasoning Question

A neural network uses the sigmoid activation function. The input to a neuron is x = 2.

- a) Calculate the output (use e ≈ 2.718)
- b) If the input were x = 10 instead, would the output be closer to 0 or 1? Explain.
- c) Why do neural networks use sigmoid instead of just the raw input x?

**Expected Output**: 
- Numeric answer for part (a)
- Written explanations for parts (b) and (c)

---

### Task 5: Application to AI (Medium)

In a softmax function for 3 classes, the raw scores are:
- Class A: 2
- Class B: 1
- Class C: 0

The softmax formula is: softmax(xᵢ) = eˣⁱ / (eˣ¹ + eˣ² + eˣ³)

- a) Calculate the softmax probability for each class (use e ≈ 2.718)
- b) Verify that the three probabilities sum to 1
- c) Which class has the highest probability? Why?
- d) What would happen if we used the raw scores directly (without eˣ) instead of softmax?

**Expected Output**: 
- Three probability values
- Verification that they sum to 1
- Written explanations for parts (c) and (d)

---

### Task 6: Understanding Growth (Medium)

Two functions represent growth:
- Function A: f(t) = 2ᵗ
- Function B: g(t) = eᵗ

- a) At t = 0, which function is larger?
- b) At t = 1, which function is larger? (use e ≈ 2.718)
- c) As t increases, which function grows faster? Explain.
- d) Why might AI systems prefer functions based on e rather than other bases?

**Expected Output**: Written answers with explanations for all four parts.

---

### Task 7: Optional Python Task

Write Python code to:
- Calculate e using: e = lim(n→∞) (1 + 1/n)ⁿ (use n = 1000000)
- Calculate eˣ for x = -2, -1, 0, 1, 2
- Implement the sigmoid function: σ(x) = 1/(1 + e⁻ˣ)
- Test sigmoid for x = -5, -2, 0, 2, 5

**Expected Output**: Python code with calculations and test outputs.

---

## Expected Output / Answer Format

For each task, provide:
- **Numeric answers**: Use e ≈ 2.718 for approximations where needed
- **Calculations**: Show your work step-by-step
- **Explanations**: Brief reasoning for conceptual questions
- **Verifications**: Check that probabilities sum correctly

**Note**: No solutions are provided—work through each problem independently!

