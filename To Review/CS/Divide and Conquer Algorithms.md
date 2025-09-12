## Paradigm Overview

**Divide-and-Conquer** is a fundamental algorithmic strategy that breaks problems into smaller subproblems, solves them recursively, and combines the solutions.

## Three-Step Process

### 1. Divide
Break the problem into several subproblems that are similar to the original problem but smaller in size.

### 2. Conquer  
Solve the subproblems recursively. If the subproblems are small enough, solve them directly (base case).

### 3. Combine
Merge the solutions of the subproblems into a solution for the original problem.

## Merge Sort Example

**[[Merge Sort Algorithm]]** perfectly illustrates this paradigm:

1. **Divide:** Split n-element array into 2 subarrays of n/2 elements each
2. **Conquer:** Recursively sort the two subarrays
3. **Combine:** Merge 2 sorted subarrays into 1 sorted array

## Key Characteristics

- **Recursive structure** naturally leads to elegant solutions
- **Parallel potential** - subproblems can often be solved independently
- **Optimal complexity** for many problems (like sorting)
- **Mathematical analysis** through [[Recurrence Relations]]

## Applications

This paradigm extends far beyond sorting and appears in numerous fundamental algorithms across computer science, making it essential for understanding advanced algorithmic techniques.

---
#### Sources
[[lecture_3_sorting_algorithms_computational_cost.pdf]]
#### Class
[[Fundamentals of Computer Science]]