*Product*Theorem 2:** $A^k(v, w) =$ number of walks of length $k$ from $v$ to $w$ with $k$ edges.

A is the [[Adjacency Matrix]]. Use [[Multiplication of Matrixes]]

**Proof:** By induction on $k$. Trivially true for $k = 1$. Assume true for some $k \geq 1$. Let $N_t(v, w)$ be the number of walks from $v$ to $w$ with $t$ edges. Let $N_t(v, w; u)$ be the number of walks from $v$ to $w$ with $t$ edges whose penultimate vertex is $u$.


$$N_{k+1}(v, w) = \sum_{u \in V} N_{k+1}(v, w; u) = \sum_{u \in V} N_k(v, u)A(u, w) = \sum_{u \in V} A^k(v, u)A(u, w) = A^{k+1}(v, w)$$

This remarkable theorem connects linear algebra with graph theory, showing that powers of the [[Adjacency Matrix]] count [[Paths and Walks|walks]] of specific lengths.

---

Key applications:
- Computing reachability in $k$ steps
- Analyzing connectivity properties
- Understanding [[Walk Length]] distributions
- Connection to [[Connected Components]] through matrix properties

The result provides a computational method for analyzing graph structure through matrix operations.

---
#### Sources:
[[lecture_2_graphs_2.pdf]]
#### Lesson:
[[Fundamentals of Computer Science]]