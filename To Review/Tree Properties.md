**Corollary 1:** If a tree $T$ has $n$ vertices then 
(a) It has $n - 1$ edges. 
(b) It has at least 2 vertices of degree 1, $(n \geq 2)$.

**Proof:** (a) is part (c) of previous lemma. $k = 1$ since $T$ is connected.

(b) Let $s$ be the number of vertices of degree 1 in $T$. There are no vertices of degree 0 – these would form separate components. Thus 
$$2n - 2 = \sum_{v \in V} d_T(v) \geq 2(n - s) + s$$
So $s \geq 2$.

These fundamental properties of [[Trees Definition|trees]] follow from their connected and acyclic nature:

- The edge count formula $|E| = |V| - 1$ is minimal for connectivity
- Leaf vertices (degree 1) must exist as "endpoints" of the tree structure
- The proof uses the [[Handshaking Lemma]] applied to trees

These results are essential for understanding tree structure and are used in [[Tree Equivalence]] characterizations.

---
#### Sources:
[[lecture_2_graphs_2.pdf]]
#### Lesson:
[[Fundamentals of Computer Science]]