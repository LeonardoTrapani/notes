**Lemma 1:** Suppose $W$ is a [[Paths and Walks|walk]] from vertex $a$ to vertex $b$ and that $W$ minimises $\ell$ over all walks from $a$ to $b$. Then $W$ is a path.

**Proof:** Suppose $W = (a = a_0, a_1, \ldots, a_k = b)$ and $a_i = a_j$ where $0 \leq i < j \leq k$. Then $W' = (a_0, a_1, \ldots, a_i, a_{j+1}, \ldots, a_k)$ is also a walk from $a$ to $b$ and $\ell(W') = \ell(W) - (j - i) < \ell(W)$ – contradiction.

_Proof in simple terms:_ assume that W is the shortest walk but NOT a path. That would mean some vertexes appear twice ($a_i = a_j$ in the proof). Then we can remove the things in between $a_{i}$ and $a_{j}$, and that would be faster.

**Corollary 1:** If $a \sim b$ then there is a path from $a$ to $b$. So $G$ is connected $\Leftrightarrow \forall a, b \in V$ there is a path from $a$ to $b$.

This fundamental result shows that shortest connections between vertices are always [[Paths and Walks|paths]] (no repeated vertices), and establishes the equivalence between connectivity via walks and connectivity via paths.

---

Essential for understanding [[Connected Graphs]] and implementing efficient algorithms like [[Breadth First Search]] for finding shortest paths.

---
#### Sources:
[[lecture_2_graphs_2.pdf]]
#### Lesson:
[[Fundamentals of Computer Science]]