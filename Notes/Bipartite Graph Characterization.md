**Theorem 1:** $G$ is bipartite $\Leftrightarrow G$ has no cycles of odd length.

**Proof:** 

$\Rightarrow$: $G = (X \cup Y, E)$. Suppose $C = (u_1, u_2, \ldots, u_k, u_1)$ is a cycle. Suppose $u_1 \in X$. Then $u_2 \in Y, u_3 \in X, \ldots, u_k \in Y$ implies $k$ is even.

$\Leftarrow$ Assume $G$ is connected, else apply following argument to each component. Choose $v \in V$ and construct $A_0, A_1, A_2, \ldots$ by [[Breadth First Search]].

$X = A_0 \cup A_2 \cup A_4 \cup \cdots$ and $Y = A_1 \cup A_3 \cup A_5 \cup \cdots$

We need only show that $X$ and $Y$ contain no edges and then all edges must join $X$ and $Y$. Suppose $X$ contains edge $(a,b)$ where $a \in A_k$ and $b \in A_\ell$.

**(i)** If $k \neq \ell$ then $|k - \ell| \geq 2$ which contradicts BFS construction.

**(ii)** $k = \ell$: There exist paths $(v = v_0, v_1, v_2, \ldots, v_k = a)$ and $(v = w_0, w_1, w_2, \ldots, w_k = b)$. Let $j = \max\{t : v_t = w_t\}$. $(v_j, v_{j+1}, \ldots, v_k, w_k, w_{k-1}, \ldots, w_j)$ is an odd cycle – length $2(k - j) + 1$ – contradiction.

This theorem provides the fundamental characterization of [[Bipartite Graphs]] in terms of [[Closed Walks and Cycles|cycles]]. The proof elegantly uses [[Breadth First Search]] to construct the bipartition when no odd cycles exist.

---

###  AI Generated Visualization
https://claude.ai/public/artifacts/9543d87e-5738-497d-98eb-723f97d481f0

---
#### Sources:
[[lecture_2_graphs_2.pdf]]
#### Lesson:
[[Fundamentals of Computer Science]]