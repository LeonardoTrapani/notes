## Θ-notation (Theta Notation)

### Mathematical Definition
$f(n) = \Theta(g(n))$: there exist positive constants $c_1$, $c_2$, and $n_0$ such that

$$0 \leq c_1 g(n) \leq f(n) \leq c_2 g(n) \text{ for all } n \geq n_0$$

### Practical Approach
For practitioners:
- **Drop low-order terms**
- **Ignore leading constants**

**Example:** $3n^3 + 90n^2 - 5n + 6046 = \Theta(n^3)$

## Asymptotic Performance Comparison

When $n$ gets large enough, a $\Theta(n^2)$ algorithm **always beats** a $\Theta(n^3)$ algorithm.

### Important Considerations
- **Don't ignore asymptotically slower algorithms** entirely
- **Real-world design** often requires careful balancing of engineering objectives  
- **Asymptotic analysis** is a useful tool to structure thinking, not the only consideration

## Key Principle

Asymptotic notation provides a framework for comparing algorithm efficiency by focusing on the **dominant growth factor** rather than implementation-specific constants or lower-order terms.

This notation is fundamental for understanding [[Algorithm Complexity Classes]] and comparing different [[Sorting Algorithms Comparison|algorithmic approaches]].

---
#### Sources
[[lecture_3_sorting_algorithms_computational_cost.pdf]]
#### Class
[[Fundamentals of Computer Science]]