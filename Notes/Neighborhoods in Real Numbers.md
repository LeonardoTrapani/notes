## Neighborhoods in Real Numbers

### Neighborhood Definition

For $x_0 \in \mathbb{R}$ and radius $r > 0$, the **neighborhood of $x_0$ with radius $r$** is:

$$N_r(x_0) = \{x \in \mathbb{R} : d(x, x_0) < r\}$$

This can be rewritten as:
$$N_r(x_0) = \{x \in \mathbb{R} : |x - x_0| < r\}$$

### Interval Representation

The condition $d(x, x_0) < r$ means $|x - x_0| < r$, which is equivalent to:
$$-r < x - x_0 < r$$

Therefore: $x_0 - r < x < x_0 + r$

So the neighborhood becomes:
$$N_r(x_0) = (x_0 - r, x_0 + r)$$

This is an **open interval** with extremes excluded.

### Right and Left Neighborhoods

**Right Neighborhood**: $N_r^+(x_0) = [x_0, x_0 + r)$
- Includes $x_0$ but excludes $x_0 + r$

**Left Neighborhood**: $N_r^-(x_0) = (x_0 - r, x_0]$  
- Excludes $x_0 - r$ but includes $x_0$

**Important Note**: Despite the names, $N_r^+(x_0)$ and $N_r^-(x_0)$ are **not neighborhoods** in the strict sense because extremes are not excluded. In fact, $x_0 \in N_r^+(x_0)$ and $x_0 \in N_r^-(x_0)$.

### Neighborhoods of Infinity

Even though $+\infty$ and $-\infty$ are not real numbers, we can define their neighborhoods:

**Neighborhood of $+\infty$**: $N(+\infty) = (a, +\infty)$ with $a \in \mathbb{R}$

**Neighborhood of $-\infty$**: $N(-\infty) = (-\infty, a)$ with $a \in \mathbb{R}$

Examples:
- $(-100, +\infty)$, $(3, +\infty)$, $(-20, +\infty)$
- $(-\infty, -50)$, $(-\infty, 0)$, $(-\infty, 8)$

---
#### Sources
[[Lecture_2.pdf]]
#### Class
[[Math and Statistics]]