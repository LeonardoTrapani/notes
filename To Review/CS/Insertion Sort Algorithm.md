## Algorithm Description

**Intuition:** Move smaller numbers to the left by inserting each element into its correct position within the already sorted portion.

## Pseudocode

```
INSERTION-SORT (A, n) ⊳ A[1 . . n]
for j ← 2 to n
    do key ← A[j]
       i ← j - 1
       while i > 0 and A[i] > key
           do A[i+1] ← A[i]
              i ← i - 1
       A[i+1] = key
```

## Algorithm Steps

1. **Start from position 2** (since single element is already sorted)
2. **Select current element** as `key`
3. **Scan backwards** through the sorted portion
4. **Shift elements** greater than `key` to the right
5. **Insert key** in the correct position

## Key Characteristics

- **In-place sorting:** Uses constant extra memory
- **Stable:** Preserves relative order of equal elements  
- **Online:** Can sort elements as they arrive
- **Adaptive:** Efficient on already sorted or nearly sorted data

## Notation

The pseudocode uses the notation `x ← y` to mean "assign the value y to variable x" (equivalent to `x = y` in most programming languages).

This algorithm demonstrates the fundamental technique used in many [[Sorting Algorithms Comparison|comparison-based sorting algorithms]] and serves as an introduction to [[Algorithm Analysis Methods]].

---
#### Sources
[[lecture_3_sorting_algorithms_computational_cost.pdf]]
#### Class
[[Fundamentals of Computer Science]]