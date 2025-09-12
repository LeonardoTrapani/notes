There is **no unique utility function representation** of a preference relation. Multiple utility functions can represent the same preferences.

## Monotonic Transformation Principle

If:
- $u$ is a utility function that represents a preference relation
- $f$ is a strictly increasing function

Then: $$V = f(u)$$

is also a utility function representing the **same** preference relation.

This is known as a **"monotonic transformation"**.

## Examples

### Squaring Transformation
For $u(x_1, x_2) = x_1 x_2$ with MRS $= -x_2/x_1$

Define $V = u^2$, so $V(x_1, x_2) = x_1^2 x_2^2$

Then: $V(2,3) = 36 > V(4,1) = V(2,2) = 16$

This gives the same preference ordering: $(2,3) \succ (4,1) \sim (2,2)$

### Linear Transformation  
Define $W = 2u + 10$, so $W(x_1, x_2) = 2x_1 x_2 + 10$

Then: $W(2,3) = 22 > W(4,1) = W(2,2) = 18$

Again, same preference ordering preserved.

## Key Implication for MRS

**Crucial Property**: The [[Marginal Rate of Substitution]] is **unchanged** by positive monotonic transformations.

For any strictly increasing function $f$, if $V = f(u)$, then:
$$\text{MRS}_V = \text{MRS}_u$$

This means the MRS captures an invariant property of preferences that doesn't depend on the specific utility representation chosen.

## Practical Significance

Since only ordinal information matters (see [[Ordinal vs Cardinal Utility]]), we can choose the most convenient utility function representation for any given problem while preserving all essential preference information.

---
#### Sources
[[MicroChapter4.pdf]]
#### Class
[[Microeconomics]]