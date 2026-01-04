# Day 1 — Probability Basics

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Probability | Learn what probability means and how to express it numerically |
| 2 | Calculate Basic Probabilities | Master the fundamental probability formula: favorable outcomes / total outcomes |
| 3 | Apply Probability to AI | Understand why probability is crucial for machine learning and AI systems |

---

## 1. Introduction

### What is Probability?

Probability is a way to measure how likely something is to happen. It's expressed as a number between 0 and 1 (or 0% and 100%).

- **0** means something will never happen (impossible)
- **1** means something will definitely happen (certain)
- **0.5** means something has a 50-50 chance (equally likely)

### Why Probability Matters for AI

In AI and machine learning, probability is everywhere:

- **Classification**: "What's the probability this email is spam?" (0.95 = 95% spam)
- **Recommendation Systems**: "What's the probability this user will like this movie?"
- **Natural Language Processing**: "What's the probability the next word is 'the'?"
- **Neural Networks**: Many AI models output probabilities for different classes

### Real-World Analogy

Think of probability like weather forecasting:
- If a meteorologist says "70% chance of rain," they're using probability
- AI systems do the same thing: "70% chance this image is a cat"

---

## 2. Deep-Dive Explanation

### The Basic Probability Formula

```
Probability = (Number of favorable outcomes) / (Total number of possible outcomes)
```

Or in mathematical notation:
```
P(Event) = Favorable Outcomes / Total Outcomes
```

### Key Concepts

**Sample Space**: All possible outcomes
- Example: Rolling a die → Sample space = {1, 2, 3, 4, 5, 6}

**Event**: A specific outcome or set of outcomes we're interested in
- Example: "Rolling an even number" → Event = {2, 4, 6}

**Probability Value**: Always between 0 and 1
- Can be written as:
  - Decimal: 0.5
  - Fraction: 1/2
  - Percentage: 50%

### Visual Representation

```
Sample Space (All Outcomes)
┌─────────────────────────┐
│ 1  2  3  4  5  6        │
└─────────────────────────┘
         │
         │ Favorable outcomes
         ▼
    ┌─────────┐
    │ 2  4  6 │  ← Event: Even numbers
    └─────────┘
    
Probability = 3 favorable / 6 total = 0.5 (50%)
```

---

## 3. Instructor Examples

### Example 1: Coin Flip

**Question**: What's the probability of getting heads when flipping a fair coin?

**Solution**:
- Total outcomes: {Heads, Tails} = 2 outcomes
- Favorable outcomes: {Heads} = 1 outcome
- Probability = 1/2 = 0.5 = 50%

**AI Connection**: Coin flips are used in AI for:
- Random initialization of neural network weights
- Stochastic gradient descent (random sampling)
- Monte Carlo simulations

---

### Example 2: Deck of Cards

**Question**: What's the probability of drawing a heart from a standard 52-card deck?

**Solution**:
- Total outcomes: 52 cards
- Favorable outcomes: 13 hearts (A, 2, 3, 4, 5, 6, 7, 8, 9, 10, J, Q, K)
- Probability = 13/52 = 1/4 = 0.25 = 25%

**AI Connection**: Card games are used to train AI agents:
- Poker AI uses probability to calculate winning chances
- Reinforcement learning agents learn optimal strategies

---

### Example 3: Spam Email Detection

**Question**: An AI system analyzed 1000 emails and found 200 were spam. What's the probability a random email is spam?

**Solution**:
- Total outcomes: 1000 emails
- Favorable outcomes (spam): 200 emails
- Probability = 200/1000 = 0.2 = 20%

**AI Connection**: This is exactly how spam filters work:
- They calculate P(spam | email content)
- If probability > threshold (e.g., 0.5), email is classified as spam

---

### Example 4: Weather Prediction

**Question**: In a dataset of 365 days, it rained on 73 days. What's the probability of rain on any given day?

**Solution**:
- Total outcomes: 365 days
- Favorable outcomes (rainy days): 73 days
- Probability = 73/365 = 0.2 = 20%

**AI Connection**: Weather prediction models use historical probability data combined with current conditions to forecast weather.

---

## 4. Summary / Key Takeaways

- ✅ Probability measures likelihood on a scale from 0 (impossible) to 1 (certain)
- ✅ Basic formula: Probability = Favorable Outcomes / Total Outcomes
- ✅ Probability is fundamental to AI: classification, predictions, and decision-making
- ✅ Can be expressed as decimal, fraction, or percentage
- ✅ Sample space = all possible outcomes; Event = what we're interested in

