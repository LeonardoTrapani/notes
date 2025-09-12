## Formal Problem Definition

**Input:** sequence $\langle a_1, a_2, \ldots, a_n \rangle$ of numbers

**Output:** permutation $\langle a'_1, a'_2, \ldots, a'_n \rangle$ such that $a'_1 \leq a'_2 \leq \cdots \leq a'_n$

The sorting problem is one of the fundamental computational problems, requiring the rearrangement of input elements into non-decreasing order.

## Key Properties

- The output must be a **permutation** (rearrangement) of the input
- The ordering constraint ensures $a'_i \leq a'_{i+1}$ for all valid indices
- This is a well-defined computational problem with clear input/output specifications

This fundamental problem serves as the foundation for studying different [[Sorting Algorithms Comparison|sorting algorithms]] and their [[Computational Complexity Analysis|computational complexity]].

---
#### Sources
[[lecture_3_sorting_algorithms_computational_cost.pdf]]
#### Class
[[Fundamentals of Computer Science]]