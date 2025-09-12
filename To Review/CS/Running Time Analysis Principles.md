## Fundamental Principles

### Input Dependency
The running time depends on the input characteristics:
- An already sorted sequence is easier to sort
- Input size significantly affects performance

### Size Parametrization
- **Parametrize running time by input size** since short sequences are easier to sort than long ones
- Focus on how performance scales with input size $n$

### Upper Bound Focus
- **Generally seek upper bounds** on running time because everybody likes a guarantee
- Upper bounds provide worst-case performance guarantees

## Key Insight: Machine Independence

### The Problem with Machine-Dependent Analysis
Running time depends on computer speed:
- **Relative speed** (on the same machine)
- **Absolute speed** (on different machines)

### Big Idea: Machine-Independent Analysis
- **Ignore machine-dependent constants** (consider conventional unit cost for elementary operations)
- **Look at growth of $T(n)$ as $n \to \infty$**
- This approach is called **"Asymptotic Analysis"**

This framework enables meaningful comparison of algorithms across different computing platforms and forms the foundation for [[Asymptotic Notation]] and [[Algorithm Complexity Classes]].

---
#### Sources
[[lecture_3_sorting_algorithms_computational_cost.pdf]]
#### Class
[[Fundamentals of Computer Science]]