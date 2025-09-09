We define a relation $\sim$ on $V$. $a \sim b$ iff there is a walk from $a$ to $b$. 

**Claim:** $\sim$ is an equivalence relation.

**Reflexivity:** $v \sim v$ as $v$ is a (trivial) walk from $v$ to $v$.

**Symmetry:** $u \sim v$ implies $v \sim u$. $(u = u_1, u_2, \ldots, u_k = v)$ is a walk from $u$ to $v$ implies $(u_k, u_{k-1}, \ldots, u_1)$ is a walk from $v$ to $u$.

**Transitivity:** $u \sim v$ and $v \sim w$ implies $u \sim w$.

This equivalence relation partitions the vertex set into disjoint connected components, where vertices in the same component are reachable from each other via [[Paths and Walks]].

The concept is essential for understanding [[Connected Graphs]] and analyzing the overall structure of a [[Simple Graph]].

---
#### Sources:
[[lecture_2_graphs_2.pdf]]
#### Lesson:
[[Fundamentals of Computer Science]]