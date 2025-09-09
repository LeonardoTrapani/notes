**Theorem 1**: 
$$\sum_{v \in V} d_G(v) = 2|E|$$

**Proof**: Consider the [[Incidence Matrix]] $M$. Row $v$ has $d_G(v)$ 1's ([[Vertex Degrees]]), so the total number of 1's in matrix $M$ is $\sum_{v \in V} d_G(v)$. Column $e$ has exactly 2 1's, so the total number of 1's in matrix $M$ is $2|E|$. □

[[Corollary - Odd Degree Vertices]]

_In simple terms_: in an incidence matrix each column has two 1's every time (connected to two edges), and each row has the degree, so the sum of all degrees of the vertices is two times the number of edges

---
#### Sources:
[[lecture_2_graphs_1.pdf]]
#### Lesson:
[[Fundamentals of Computer Science]]