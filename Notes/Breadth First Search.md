Fix $v \in V$. For $w \in V$ let $$d(v, w) = \text{length of shortest path from } v \text{ to } w$$

For $t = 0, 1, 2, \ldots$, let $$A_t = \{w \in V : d(v, w) = t\}$$

In BFS we construct $A_0, A_1, A_2, \ldots$ by 
$$A_{t+1} = \{w \notin A_0 \cup A_1 \cup \cdots \cup A_t : \exists \text{ an edge } (u,w) \text{ such that } u \in A_t\}$$

**Note:** no edges $(a,b)$ between $A_k$ and $A_\ell$ for $\ell - k \geq 2$, else $w \in A_{k+1} \neq A_\ell$. 

$A_0 = \{v\}$ and $v \sim w \Leftrightarrow d(v, w) < \infty$.

BFS systematically explores vertices layer by layer, finding shortest paths from a source vertex. It's fundamental for analyzing [[Connected Graphs]] and determining [[Connected Components]].

The algorithm guarantees that paths found are shortest due to the [[Shortest Path Lemma]], and the layered structure $A_t$ contains all vertices at distance exactly $t$ from the source.

Used in the proof of [[Bipartite Graph Characterization]] to construct the two-coloring of bipartite graphs.

---
#### Sources:
[[lecture_2_graphs_2.pdf]]
#### Lesson:
[[Fundamentals of Computer Science]]