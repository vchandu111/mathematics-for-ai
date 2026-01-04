# Day 4 — Integration in Python

## Learning Objectives

| # | Learning Objective | Description |
| - | ------------------ | ----------- |
| 1 | Use scipy.integrate | Learn to calculate integrals numerically in Python |
| 2 | Understand Numerical Methods | See how Python approximates integrals |
| 3 | Apply to AI Problems | Use Python integration for probability and optimization |

---

## 1. Introduction

### Why Python for Integration?

While we can calculate integrals by hand, Python helps us:
- **Handle Complex Functions**: Functions that are hard to integrate analytically
- **Numerical Accuracy**: Get precise approximations
- **Automation**: Calculate many integrals quickly
- **Visualization**: Plot functions and their integrals

### Why This Matters for AI

In AI, we often need to:
- **Calculate Probabilities**: Integrate probability density functions
- **Expected Values**: Integrate x·f(x) for continuous distributions
- **Loss Functions**: Integrate complex loss functions
- **Performance Metrics**: Calculate areas under curves (like AUC-ROC)

### Real-World Analogy

Think of Python integration like a calculator:
- **By Hand**: You can do arithmetic, but it's slow
- **Calculator**: Fast, accurate, handles complex calculations
- **Python**: Like a super-calculator that can do thousands of integrals instantly

---

## 2. Deep-Dive Explanation

### Using scipy.integrate.quad

The `quad` function calculates definite integrals numerically:

```python
from scipy.integrate import quad

result, error = quad(function, a, b)
```

- `function`: The function to integrate (as a Python function)
- `a, b`: Lower and upper bounds
- Returns: `(result, error)` - the integral value and estimated error

### Basic Example

```python
from scipy.integrate import quad
import numpy as np

def f(x):
    return x**2

result, error = quad(f, 0, 3)
print(f"Integral: {result}")  # Should be approximately 9
```

### For Polynomials: numpy.polyint

For polynomials, we can also use symbolic integration:

```python
import numpy as np

# Coefficients of x²: [1, 0, 0] means 1·x² + 0·x + 0
coeffs = [1, 0, 0]  # for x²
antiderivative = np.polyint(coeffs)  # [1/3, 0, 0, 0] for x³/3
```

---

## 3. Instructor Examples

### Example 1: Simple Definite Integral

**Question**: Calculate ∫[0 to 3] x² dx using Python.

**Solution**:
```python
from scipy.integrate import quad

def f(x):
    return x**2

result, error = quad(f, 0, 3)
print(f"Integral: {result:.2f}")  # Output: 9.00
```

**AI Connection**: This is how we'd calculate probabilities or expected values in machine learning models programmatically.

---

### Example 2: Probability Calculation

**Question**: For probability density f(x) = 2x on [0, 1], calculate P(0 ≤ X ≤ 0.5).

**Solution**:
```python
from scipy.integrate import quad

def pdf(x):
    return 2 * x

probability, error = quad(pdf, 0, 0.5)
print(f"Probability: {probability:.4f}")  # Output: 0.2500
```

**AI Connection**: This is exactly how we calculate probabilities for continuous random variables in Python-based ML models.

---

### Example 3: Expected Value

**Question**: Calculate E[X] = ∫[0 to 1] x·(2x) dx for f(x) = 2x.

**Solution**:
```python
from scipy.integrate import quad

def expected_value_integrand(x):
    return x * (2 * x)  # x * f(x)

expected_value, error = quad(expected_value_integrand, 0, 1)
print(f"Expected Value: {expected_value:.4f}")  # Output: 0.6667
```

**AI Connection**: Expected values are crucial for understanding average model outputs, average prediction scores, etc.

---

### Example 4: Complex Function

**Question**: Calculate ∫[0 to 1] e⁻ˣ dx (this is harder to do by hand).

**Solution**:
```python
from scipy.integrate import quad
import numpy as np

def f(x):
    return np.exp(-x)

result, error = quad(f, 0, 1)
print(f"Integral: {result:.6f}")  # Approximately 0.632121
```

**AI Connection**: Many AI models use exponential functions (like in sigmoid, softmax). Python integration handles these easily.

---

## 4. Summary / Key Takeaways

- ✅ **scipy.integrate.quad**: Main function for numerical integration
- ✅ **Syntax**: `quad(function, a, b)` returns `(result, error)`
- ✅ **Useful for**: Complex functions, probability calculations, expected values
- ✅ **AI Applications**: Probability densities, loss functions, performance metrics
- ✅ Python makes integration practical for real AI applications

