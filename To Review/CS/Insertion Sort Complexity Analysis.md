## Worst Case Analysis

**Scenario:** Input reverse sorted

**Time Complexity:** 
$$T(n) = \sum_{j=2}^{n} \Theta(j) = \Theta(n^2)$$

This follows from the arithmetic series formula (discovered by Gauss at 6 years old).

## Average Case Analysis

**Assumption:** All permutations equally likely

**Time Complexity:** 
$$T(n) = \sum_{j=2}^{n} \Theta(j/2) = \Theta(n^2)$$

The average case has the same asymptotic complexity as the worst case, differing only by a constant factor.

## Performance Assessment

### Is insertion sort fast?
- **Moderately so, for small $n$**
- **Not at all, for large $n$**

## Key Insights

1. **Both worst and average cases are $\Theta(n^2)$**
2. **Quadratic growth** makes it impractical for large datasets
3. **Reasonable performance** for small inputs (typically $n < 30$)
4. The algorithm's simplicity makes it useful despite quadratic complexity

This analysis demonstrates why more efficient algorithms like [[Merge Sort Algorithm]] are needed for large-scale sorting problems, leading to the study of [[Divide and Conquer Algorithms]].

---
#### Sources
[[lecture_3_sorting_algorithms_computational_cost.pdf]]
#### Class
[[Fundamentals of Computer Science]]