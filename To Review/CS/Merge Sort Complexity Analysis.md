## Recurrence Relation

The time complexity of merge sort can be expressed as:

$$T(n) = \begin{cases} 
\Theta(1) & \text{if } n = 1 \\
2T(n/2) + \Theta(n) & \text{if } n > 1
\end{cases}$$

### Component Analysis
- **Base case:** $\Theta(1)$ for single element
- **Recursive calls:** $2T(n/2)$ for sorting two halves  
- **Merge operation:** $\Theta(n)$ for combining results

## Recursion Tree Method

### Tree Structure
- **Height:** $h = \lg n$
- **Work per level:** $cn$ (where $c$ is a constant)
- **Number of levels:** $\lg n + 1$
- **Leaves:** $n$ nodes, each requiring $\Theta(1)$ work

### Total Complexity Calculation
$$\text{Total} = \underbrace{cn \times (\lg n + 1)}_{\text{internal nodes}} + \underbrace{\Theta(n)}_{\text{leaves}} = \Theta(n \lg n)$$

## Key Result

**Merge sort achieves $\Theta(n \lg n)$ time complexity** in all cases (worst, average, and best).

## Practical Implications

- **$\Theta(n \lg n)$ grows more slowly than $\Theta(n^2)$**
- **Merge sort asymptotically beats [[Insertion Sort Algorithm]]** in worst case
- **In practice,** merge sort beats insertion sort for $n > 30$ or so

## Note on Recurrence Simplification

The textbook (CLRS) provides several methods for solving such recurrences. We typically omit the base case when $T(n) = \Theta(1)$ for small $n$ when it doesn't affect the asymptotic solution.

This analysis demonstrates the power of [[Recurrence Relations]] and shows why [[Divide and Conquer Algorithms]] often achieve optimal complexity.

---
#### Sources
[[lecture_3_sorting_algorithms_computational_cost.pdf]]
#### Class
[[Fundamentals of Computer Science]]