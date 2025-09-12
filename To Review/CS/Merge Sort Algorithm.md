## Algorithm Overview

**Merge Sort** is a recursive sorting algorithm that follows the divide-and-conquer paradigm.

## Algorithm Steps

```
MERGE-SORT A[1 . . n]
1. If n = 1, done.
2. Recursively sort A[1 . . ⌈n/2⌉] and A[⌈n/2⌉+1 . . n].
3. "Merge" the 2 sorted lists.
```

## Elegant Recursive Pseudocode

```
MERGE-SORT (A[1 . . n])
{ if n > 1
    MERGE-SORT (A[1 . . ⌈n/2⌉])
    MERGE-SORT (A[⌈n/2⌉+1 . . n])
    MERGE(A[1 . . n])
}
```

## Divide-and-Conquer Strategy

1. **Divide:** Split the n-element array A into 2 subarrays of n/2 elements each
2. **Conquer:** Recursively sort the two subarrays  
3. **Combine:** Merge 2 sorted subarrays into 1 sorted array

## Key Subroutine

The **MERGE** operation is the critical component that combines two sorted arrays in linear time. The merge process takes $\Theta(n)$ time to merge a total of n elements.

## Advantages

- **Guaranteed $O(n \log n)$ performance** in all cases
- **Stable sorting** preserves relative order of equal elements
- **Predictable performance** regardless of input distribution
- **Recursive structure** makes it elegant and easy to analyze

The merge sort algorithm demonstrates the power of [[Divide and Conquer Algorithms]] and leads to the study of [[Recurrence Relations]] for analyzing recursive algorithms.

---
#### Sources
[[lecture_3_sorting_algorithms_computational_cost.pdf]]
#### Class
[[Fundamentals of Computer Science]]