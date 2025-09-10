## Definition

If:
- $u$ is a [[Utility Functions|utility function]] that represents a preference relation, and
- $f$ is a **strictly increasing function**

Then $V = f(u)$ is also a utility function representing the **same preference relation**.

This is known as a **monotonic transformation**.

## Mathematical Examples

### Transformation 1: Squaring
Starting with $u(x_1, x_2) = x_1 x_2$:
- $V = u^2$, so $V(x_1, x_2) = x_1^2 x_2^2$
- For bundles $(2,3)$, $(4,1)$, $(2,2)$:
  - $V(2,3) = 36 > V(4,1) = V(2,2) = 16$
- Same preference ordering: $(2,3) \succ (4,1) \sim (2,2)$

### Transformation 2: Linear Transformation  
Using the same base utility function:
- $W = 2u + 10$, so $W(x_1, x_2) = 2x_1 x_2 + 10$
- For the same bundles:
  - $W(2,3) = 22 > W(4,1) = W(2,2) = 18$
- Same preference ordering preserved

## Key Properties

### Preference Preservation
Monotonic transformations preserve:
- **Preference ordering** between bundles
- **Indifference relationships** between bundles
- The underlying preference structure

### MRS Invariance
Importantly, monotonic transformations **do not change** the [[Marginal Rate of Substitution]]:
- The MRS remains the same across all monotonic transformations
- This makes MRS a robust measure independent of utility function scaling

## General Principle

Since [[Ordinal vs Cardinal Utility|utility is ordinal]], any strictly increasing transformation represents the same preferences. This reflects that:
- The absolute scale of utility is arbitrary
- Only the relative ranking matters
- Different utility functions can represent identical preference relations

---
#### Sources
[[MicroChapter4.pdf]]
#### Class
[[Microeconomics]]