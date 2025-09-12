## Monotonic Transformations and Demand Equivalence

### Key Insight from Cobb-Douglas Examples

Consider these three apparently different utility functions:

1. $U(x_1, x_2) = x_1^{1/2}x_2^{1/2}$
2. $U(x_1, x_2) = x_1x_2$ 
3. $U(x_1, x_2) = \ln x_1 + \ln x_2$

### Identical Demand Functions

Despite their different forms, all three yield the **same demand functions**:
$$x_1(p_1, p_2, m) = \frac{1}{2}\frac{m}{p_1}$$
$$x_2(p_1, p_2, m) = \frac{1}{2}\frac{m}{p_2}$$

### Explanation: Monotonic Transformations

These utility functions are **monotonic transformations** of each other:
- Function 2 is the square of function 1: $(x_1^{1/2}x_2^{1/2})^2 = x_1x_2$
- Function 3 is the natural log of function 2: $\ln(x_1x_2) = \ln x_1 + \ln x_2$

### Theoretical Foundation

#### Ordinal Nature of Utility
Since [[Ordinal vs Cardinal Utility|utility is ordinal]], any monotonic transformation preserves the preference ordering and therefore yields identical optimal choices.

#### Mathematical Reason
Monotonic transformations preserve the [[Marginal Rate of Substitution|MRS]]:
$$MRS = \frac{MU_{x_1}}{MU_{x_2}} = \frac{x_2}{x_1}$$

This ratio remains unchanged across all three representations.

### Practical Implication

**Time-Saving Principle**: If you recognize that utility functions are monotonic transformations of each other, you only need to derive the demand functions once.

### General Cobb-Douglas Pattern

For any Cobb-Douglas utility function $U(x_1, x_2) = x_1^a x_2^b$ (or its monotonic transformations):

$$x_1(p_1, p_2, m) = \frac{a}{a+b}\frac{m}{p_1}$$
$$x_2(p_1, p_2, m) = \frac{b}{a+b}\frac{m}{p_2}$$

### Connection to Other Preference Types
This principle applies broadly:
- Different representations of [[Perfect Complements Utility Function|perfect complements]]
- Various forms of [[Perfect Substitutes Utility Function|perfect substitutes]]  
- Alternative formulations of [[Quasi-Linear Utility Function|quasi-linear preferences]]

---
#### Sources
[[MicroChapter5.pdf]]
#### Class
[[Microeconomics]]