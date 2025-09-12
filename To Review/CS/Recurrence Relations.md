## Definition

A **recurrence relation** expresses a function in terms of its values on smaller inputs, providing a mathematical framework for analyzing recursive algorithms.

## General Form

For divide-and-conquer algorithms:
$$T(n) = \begin{cases}
\text{base case} & \text{if } n \leq n_0 \\
\text{combination of } T(\text{smaller inputs}) + \text{work at current level} & \text{otherwise}
\end{cases}$$

## Merge Sort Example

$$T(n) = \begin{cases}
\Theta(1) & \text{if } n = 1 \\
2T(n/2) + \Theta(n) & \text{if } n > 1
\end{cases}$$

This recurrence captures:
- **Base case:** Constant time for trivial problem
- **Recursive structure:** Two subproblems of half the size
- **Combination cost:** Linear time to merge results

## Solution Method: Recursion Tree

**Solve $T(n) = 2T(n/2) + cn$ where $c > 0$ is constant:**

1. **Tree height:** $h = \lg n$
2. **Work per level:** $cn$ (constant across all levels)
3. **Total levels:** $\lg n + 1$
4. **Leaf contribution:** $\Theta(n)$

**Solution:** $T(n) = \Theta(n \lg n)$

## Key Insights

- Recurrences provide **precise complexity analysis** for recursive algorithms
- **Recursion tree method** visualizes the work distribution across recursion levels
- Many divide-and-conquer algorithms follow similar recurrence patterns

## Simplification Convention

We typically omit base case details when $T(n) = \Theta(1)$ for sufficiently small $n$, provided it doesn't affect the asymptotic solution.

This mathematical framework is essential for analyzing [[Divide and Conquer Algorithms]] and understanding why algorithms like [[Merge Sort Algorithm]] achieve optimal performance.

---
#### Sources
[[lecture_3_sorting_algorithms_computational_cost.pdf]]
#### Class
[[Fundamentals of Computer Science]]