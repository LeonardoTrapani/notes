The equivalence classes of $\sim$ are called **connected components**. In general $V = C_1 \cup V_2 \cup \cdots \cup C_r$ where $C_1, C_2, \ldots, C_r$ are the connected components. We let $\omega(G)(= r)$ be the number of components of $G$. 

$G$ is **connected** iff $\omega(G) = 1$ i.e. there is a walk between every pair of vertices. Thus $C_1, C_2, \ldots, C_r$ induce connected subgraphs $G[C_1], \ldots, G[C_r]$ of $G$.

A connected graph is one where every vertex can reach every other vertex through some sequence of edges. This is fundamental for many graph algorithms and properties.

---

Key relationships:
- Connected components form [[Induced Subgraph|induced subgraphs]]
- [[Trees Definition|Trees]] are connected graphs without cycles  
- [[Breadth First Search]] can be used to explore connected components
- The relation is based on [[Connected Components]] equivalence classes

---
#### Sources:
[[lecture_2_graphs_2.pdf]]
#### Lesson:
[[Fundamentals of Computer Science]]