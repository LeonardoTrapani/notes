## Worst-Case Analysis (Usually)

**Definition:** $T(n) = $ maximum time of algorithm on any input of size $n$

- Most commonly used in practice
- Provides guaranteed performance bounds
- Essential for critical applications

## Average-Case Analysis (Sometimes)

**Definition:** $T(n) = $ expected time of algorithm over all inputs of size $n$

**Requirements:**
- Needs assumption of statistical distribution of inputs
- More complex to analyze
- Useful when input distribution is known

## Best-Case Analysis (Bogus)

**Why it's problematic:**
- Can cheat with a slow algorithm that works fast on some specific input
- Doesn't provide meaningful performance guarantees
- Generally not useful for practical algorithm evaluation

## Analysis Choice Guidelines

- **Worst-case:** Preferred for most practical applications
- **Average-case:** Valuable when input patterns are well-understood
- **Best-case:** Generally avoided as misleading

The choice of analysis type significantly impacts how we evaluate and compare different [[Sorting Algorithms Comparison|sorting algorithms]] and their practical utility.

---
#### Sources
[[lecture_3_sorting_algorithms_computational_cost.pdf]]
#### Class
[[Fundamentals of Computer Science]]