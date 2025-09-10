# Paths and Connectivity Flashcards

Source: [[Graph Theory Index]]
Tags: #flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

## Walks and Paths
What is a walk $W = (v_1, v_2, \ldots, v_k)$ in graph $G$?::A sequence of vertices where $(v_i, v_{i+1}) \in E$ for $1 \leq i < k$ (consecutive vertices are connected by edges)
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

What is a path?::A walk in which all vertices are distinct (no repeated vertices)
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

What is the difference between a walk and a path?::A walk can repeat vertices and edges, while a path has all distinct vertices
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

## Walk Length
What is the length $\ell(W)$ of a walk $W$?::The number of edges in $W$ (regardless of whether vertices or edges are repeated)
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

## Closed Walks and Cycles
What is a closed walk?::A walk where $v_1 = v_k$ (starts and ends at the same vertex)
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

What is a cycle?::A closed walk in which all vertices are distinct except for $v_1 = v_k$ (start/end vertex)
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

What is the key difference between a closed walk and a cycle?::A cycle is the simplest form of closed walk where no vertex is repeated except the start/end vertex
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

## Connected Components
In graph theory, when do we say $a \sim b$ for vertices $a$ and $b$?::When there is a walk from $a$ to $b$
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

Why is the relation $\sim$ (reachability) an equivalence relation?::Reflexive: $v \sim v$ (trivial walk), Symmetric: walk from $u$ to $v$ implies walk from $v$ to $u$ (reverse), Transitive: $u \sim v$ and $v \sim w$ implies $u \sim w$ (concatenate walks)
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

What are connected components?::The equivalence classes of the reachability relation $\sim$, partitioning vertices into disjoint sets where vertices in the same set are reachable from each other
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

What is $\omega(G)$?::The number of connected components in graph $G$
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

## Connected Graphs  
When is a graph $G$ connected?::When $\omega(G) = 1$, i.e., there is a walk between every pair of vertices
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

What is an equivalent condition for graph connectivity?::For all vertices $a, b \in V$, there exists a path from $a$ to $b$
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

## Shortest Path Lemma
State the Shortest Path Lemma::If $W$ is a walk from vertex $a$ to vertex $b$ that minimizes length over all walks from $a$ to $b$, then $W$ is a path
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

Why must the shortest walk between two vertices be a path?::If the shortest walk repeated a vertex, we could remove the loop between repetitions to get a shorter walk, contradicting minimality
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

What is the corollary of the Shortest Path Lemma?::If $a \sim b$, then there is a path from $a$ to $b$. So $G$ is connected $\Leftrightarrow$ for all $a, b \in V$ there is a path from $a$ to $b$
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

## Breadth First Search
In BFS starting from vertex $v$, what is $d(v, w)$?::The length of the shortest path from $v$ to $w$
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

In BFS, what is $A_t$?::$A_t = \{w \in V : d(v, w) = t\}$ - the set of all vertices at distance exactly $t$ from the source vertex $v$
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

How does BFS construct the sets $A_{t+1}$?::$A_{t+1} = \{w \notin A_0 \cup A_1 \cup \cdots \cup A_t : \exists \text{ an edge } (u,w) \text{ such that } u \in A_t\}$
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

What is the key property about edges between different BFS levels?::No edges exist between $A_k$ and $A_\ell$ for $\ell - k \geq 2$ (vertices can only be connected to adjacent levels)
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity

In BFS, what does $A_0$ equal and what condition determines if $v \sim w$?::$A_0 = \{v\}$ (source vertex) and $v \sim w \Leftrightarrow d(v, w) < \infty$
#flashcards/fundamentals-of-computer-science/graph-theory/paths-connectivity