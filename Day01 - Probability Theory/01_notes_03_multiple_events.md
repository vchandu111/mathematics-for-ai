# Day 1 — Multiple Events

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Understand Independent Events | Learn when events don't affect each other's probability |
| 2 | Calculate Joint Probabilities | Master AND (multiplication) and OR (addition) rules |
| 3 | Apply to AI Scenarios | Understand how multiple events are used in AI decision-making |

---

## 1. Introduction

### What are Multiple Events?

When we consider more than one event happening, we need special rules to calculate probabilities. The two main scenarios are:

1. **AND** (both events happen): "What's the probability of A AND B?"
2. **OR** (at least one event happens): "What's the probability of A OR B?"

### Why Multiple Events Matter for AI

In AI systems, we often need to combine probabilities:

- **Spam Detection**: "What's the probability an email contains 'free' AND 'money'?"
- **Image Classification**: "What's the probability an image has a cat OR a dog?"
- **Recommendation Systems**: "What's the probability a user likes movie A AND movie B?"
- **Bayesian Networks**: Complex AI systems that combine multiple probability events

### Real-World Analogy

Think of multiple events like cooking:
- **AND**: "What's the chance I have eggs AND flour?" (need both)
- **OR**: "What's the chance I have eggs OR flour?" (need at least one)

---

## 2. Deep-Dive Explanation

### Independent Events

**Independent events** = Events that don't affect each other's probability.

**Key Rule**: For independent events A and B:
```
P(A AND B) = P(A) × P(B)
```

**Example**: 
- P(Heads on coin 1) = 0.5
- P(Heads on coin 2) = 0.5
- P(Heads on both) = 0.5 × 0.5 = 0.25

### The AND Rule (Multiplication)

When we want **both** events to happen:
```
P(A AND B) = P(A) × P(B)  [if independent]
```

### The OR Rule (Addition)

When we want **at least one** event to happen:
```
P(A OR B) = P(A) + P(B) - P(A AND B)
```

**Special Case**: If events are **mutually exclusive** (can't both happen):
```
P(A OR B) = P(A) + P(B)
```

### Visual Representation

```
AND (Both happen):
Event A: [████████░░] 50%
Event B: [████████░░] 50%
Both:    [████░░░░░░] 25% (0.5 × 0.5)

OR (At least one):
Event A: [████████░░] 50%
Event B: [████████░░] 50%
Either:  [██████████] 75% (0.5 + 0.5 - 0.25)
```

### Mutually Exclusive Events

**Mutually exclusive** = Events that cannot happen at the same time.

**Example**: Rolling a die
- Can't roll both a 3 AND a 5 on the same roll
- P(3 OR 5) = P(3) + P(5) = 1/6 + 1/6 = 2/6 = 1/3

---

## 3. Instructor Examples

### Example 1: Independent Coin Flips

**Question**: What's the probability of getting heads on both of two coin flips?

**Solution**:
- P(Heads on flip 1) = 0.5
- P(Heads on flip 2) = 0.5
- Events are independent (first flip doesn't affect second)
- P(Heads AND Heads) = 0.5 × 0.5 = 0.25 = 25%

**AI Connection**: Random number generation in AI often uses independent events. Each random choice is independent of previous ones.

---

### Example 2: Drawing Cards (Without Replacement)

**Question**: From a standard deck, what's the probability of drawing a heart AND then (without replacement) drawing another heart?

**Solution**:
- P(First heart) = 13/52 = 1/4
- After drawing one heart, 12 hearts remain out of 51 cards
- P(Second heart | first was heart) = 12/51
- P(Heart AND Heart) = (13/52) × (12/51) = 156/2652 = 1/17 ≈ 0.059

**Note**: These are NOT independent (second draw depends on first), so we use conditional probability.

**AI Connection**: Sequential decision-making in AI (like game-playing agents) must account for how previous actions affect future probabilities.

---

### Example 3: Mutually Exclusive Events

**Question**: What's the probability of rolling a 2 OR a 5 on a single die roll?

**Solution**:
- P(2) = 1/6
- P(5) = 1/6
- Events are mutually exclusive (can't roll both)
- P(2 OR 5) = P(2) + P(5) = 1/6 + 1/6 = 2/6 = 1/3

**AI Connection**: In classification, classes are often mutually exclusive. "Is this a cat OR a dog?" uses the OR rule.

---

### Example 4: AI Spam Detection

**Question**: An AI spam filter calculates:
- P(email contains "free") = 0.3
- P(email contains "money") = 0.2
- P(email contains both) = 0.1

What's the probability an email contains "free" OR "money"?

**Solution**:
- Using the OR rule: P(Free OR Money) = P(Free) + P(Money) - P(Free AND Money)
- = 0.3 + 0.2 - 0.1 = 0.4 = 40%

**AI Connection**: Real spam filters combine multiple word probabilities to make classification decisions.

---

## 4. Summary / Key Takeaways

- ✅ **Independent events**: P(A AND B) = P(A) × P(B)
- ✅ **OR rule**: P(A OR B) = P(A) + P(B) - P(A AND B)
- ✅ **Mutually exclusive**: If events can't both happen, P(A OR B) = P(A) + P(B)
- ✅ Multiple events are fundamental to AI: combining features, sequential decisions, and classification
- ✅ Always check if events are independent or dependent before applying rules

