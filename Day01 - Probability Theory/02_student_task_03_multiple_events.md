# Day 1 — Student Task: Multiple Events

## Instructions

Solve the following problems involving multiple events. For each problem:
1. Identify whether events are independent, dependent, or mutually exclusive
2. Determine if you need the AND rule or OR rule
3. Show your calculations
4. Provide the final probability

---

## Tasks

### Task 1: Basic AND Probability (Easy)

Two fair coins are flipped. What is the probability of getting:
- a) Heads on the first coin AND heads on the second coin?
- b) Tails on the first coin AND tails on the second coin?

**Expected Output**: Two probability values with brief explanations of why the AND rule applies.

---

### Task 2: Basic OR Probability (Easy)

A single die is rolled. What is the probability of rolling:
- a) A 1 OR a 6?
- b) An even number (2, 4, or 6) OR an odd number (1, 3, or 5)?

**Expected Output**: Two probability values. For part (b), explain why the answer makes sense.

---

### Task 3: Medium Reasoning Question

An AI system analyzes images and calculates:
- P(image contains a cat) = 0.4
- P(image contains a dog) = 0.3
- P(image contains both a cat AND a dog) = 0.1

Calculate:
- a) P(image contains a cat OR a dog)
- b) P(image contains neither a cat nor a dog)

**Expected Output**: 
- Answer to part (a) with calculation shown
- Answer to part (b) with explanation of your reasoning

---

### Task 4: Medium Reasoning Question

A machine learning model predicts user preferences:
- P(user likes action movies) = 0.6
- P(user likes comedy movies) = 0.5
- P(user likes both action AND comedy) = 0.3

Answer:
- a) What is P(user likes action OR comedy)?
- b) Are the events "likes action" and "likes comedy" independent? Explain your reasoning.

**Expected Output**: 
- Answer to part (a) with calculation
- Written explanation for part (b) with reasoning

---

### Task 5: Application to AI (Medium)

A spam detection AI analyzes emails and finds:
- 30% of emails contain the word "free"
- 25% of emails contain the word "urgent"
- 10% of emails contain both "free" AND "urgent"

The AI classifies an email as spam if it contains "free" OR "urgent".

- a) What percentage of emails will be classified as spam by this rule?
- b) If an email contains "free", what additional information would help determine if it's spam? Explain.

**Expected Output**: 
- Answer to part (a) with calculation
- Written explanation for part (b)

---

### Task 6: Independent Events (Medium)

A neural network uses random initialization where:
- Each weight has a 0.5 probability of being positive
- Each weight is independent of others

If the network has 3 weights, what is the probability that:
- a) All 3 weights are positive?
- b) At least one weight is positive?
- c) Exactly 2 weights are positive?

**Expected Output**: Three probability values with calculations shown.

---

### Task 7: Optional Python Task

Write a Python function that calculates:
- `probability_and(p_a, p_b, independent=True)` - returns P(A AND B)
- `probability_or(p_a, p_b, p_a_and_b=None)` - returns P(A OR B)

Test with:
- Independent events: P(A)=0.6, P(B)=0.4
- Overlapping events: P(A)=0.5, P(B)=0.3, P(A AND B)=0.2

**Expected Output**: Python code with functions and test cases showing outputs.

---

## Expected Output / Answer Format

For each task, provide:
- **Event identification**: State if events are independent, dependent, or mutually exclusive
- **Rule selection**: Explain whether you're using AND or OR rule
- **Calculation**: Show your work step-by-step
- **Final answer**: Probability as decimal and percentage
- **Explanation**: Brief reasoning for medium-level questions

**Note**: No solutions are provided—work through each problem independently!

