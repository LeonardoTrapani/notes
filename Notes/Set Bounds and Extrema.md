## Set Bounds and Extrema

### Infimum and Supremum

For a set $A \subseteq \mathbb{R}$:

**Infimum**: $\inf A$ is the greatest lower bound of $A$
- If $A$ has a minimum, then $\inf A = \min A$
- If $A$ has no minimum, $\inf A$ may still exist as the greatest lower bound

**Supremum**: $\sup A$ is the least upper bound of $A$  
- If $A$ has a maximum, then $\sup A = \max A$
- If $A$ has no maximum, $\sup A$ may still exist as the least upper bound

### Maximum and Minimum Functions

For $x \in \mathbb{R}$:

$$\max(x, -x) = \begin{cases}
x & \text{if } x \geq -x \\
-x & \text{if } x < -x
\end{cases}$$

This function chooses the greatest value between $x$ and $-x$.

$$\min(x, -x) = \begin{cases}
-x & \text{if } x \geq -x \\
x & \text{if } x < -x  
\end{cases}$$

This function chooses the smallest value between $x$ and $-x$.

### Bounded Sets

A set $A$ is:
- **Bounded above** if there exists $M \in \mathbb{R}$ such that $x \leq M$ for all $x \in A$
- **Bounded below** if there exists $m \in \mathbb{R}$ such that $x \geq m$ for all $x \in A$  
- **Bounded** if it is both bounded above and below

### Collection of Intervals

For a collection of intervals $\{A_m\}_{m \in \mathbb{N}}$ where $A_m = (-\frac{1}{m}, \frac{1}{m})$:

The intersection $A = \bigcap_{m} A_m$ represents the common elements in all intervals.

When $A_1 \supset A_2 \supset A_3 \supset \ldots$ (nested intervals), the intersection may be:
- A single point: $A = \{0\}$
- An interval: $A = [0,0]$
- The empty set if there's no common element

In this case: $\inf A = \min A = \sup A = \max A = 0$

---
#### Sources
[[Lecture_2.pdf]]
#### Class
[[Math and Statistics]]