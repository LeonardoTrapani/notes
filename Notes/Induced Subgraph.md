If $V' \subseteq V$ then 
$$G[V'] = (V', \{(u,v) \in E : u,v \in V'\})$$
is the [[Subgraphs|subgraph]] of $G$ induced by $V'$.

In simple terms: you select a subset of vertices, and all vertices of that subset connect to eachother

---

Similarly, if $E_1 \subseteq E$ then $G[E_1] = (V_1, E_1)$ where 
$$V_1 = \{v \in V_1 : \exists e \in E_1 \text{ such that } v \in e\}$$
is also induced (by $E_1$).

In simple terms: given a subset of edges take all all the vertices that connected them in the original graph



---
#### Sources:
[[lecture_2_graphs_1.pdf]]
#### Lesson:
[[Fundamentals of Computer Science]]