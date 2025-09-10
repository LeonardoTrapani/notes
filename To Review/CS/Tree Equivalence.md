**Theorem 1:** Suppose $|V| = n$ and $|E| = n - 1$. The following three statements become equivalent.
(a) $G$ is connected.
(b) $G$ is acyclic. 
(c) $G$ is a tree.

This equivalence theorem provides three different ways to characterize [[Trees Definition|trees]] when the edge count is exactly $n-1$:

- **Connectivity**: Every vertex can reach every other vertex
- **Acyclicity**: No [[Closed Walks and Cycles|cycles]] exist in the graph  
- **Tree property**: Satisfies both connected and acyclic conditions

The theorem shows that with exactly $n-1$ edges, any one of these properties implies the others. This is fundamental for:

- Proving tree properties without checking all conditions
- Understanding minimal connectivity requirements
- Algorithm design for tree recognition

This builds on [[Tree Properties]] and connects to [[Connected Graphs]] theory, showing that trees are precisely the minimal connected graphs.

---
#### Sources:
[[lecture_2_graphs_2.pdf]]
#### Lesson:
[[Fundamentals of Computer Science]]