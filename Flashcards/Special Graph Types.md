# Special Graph Types Flashcards

Source: [[Graph Theory Index]]
Tags: #flashcards/fundamentals-of-computer-science/graph-theory/special-types

## Bipartite Graphs
What is a bipartite graph?::A graph where $V = X \cup Y$ with $X$ and $Y$ disjoint, and every edge is of the form $(x,y)$ where $x \in X$ and $y \in Y$
#flashcards/fundamentals-of-computer-science/graph-theory/special-types

How can you describe bipartite graphs in simple terms?::Vertices can be divided into two disjoint sets such that no two vertices within the same set are adjacent
#flashcards/fundamentals-of-computer-science/graph-theory/special-types

## Bipartite Graph Characterization
State the fundamental theorem characterizing bipartite graphs::$G$ is bipartite $\Leftrightarrow$ $G$ has no cycles of odd length
#flashcards/fundamentals-of-computer-science/graph-theory/special-types

Why can't bipartite graphs have odd cycles? (Forward direction proof)::If $G = (X \cup Y, E)$ and $C = (u_1, u_2, \ldots, u_k, u_1)$ is a cycle with $u_1 \in X$, then $u_2 \in Y, u_3 \in X, \ldots$, so $u_k \in Y$, implying $k$ is even
#flashcards/fundamentals-of-computer-science/graph-theory/special-types

How does BFS prove that graphs without odd cycles are bipartite?::Construct BFS levels $A_0, A_1, A_2, \ldots$ from any vertex. Set $X = A_0 \cup A_2 \cup A_4 \cup \cdots$ and $Y = A_1 \cup A_3 \cup A_5 \cup \cdots$. No edges exist within $X$ or $Y$ because that would create odd cycles
#flashcards/fundamentals-of-computer-science/graph-theory/special-types

## Complete Graphs
What is the complete graph $K_n$?::$K_n = ([n], \{(i,j) : 1 \leq i < j \leq n\})$ - a graph on $n$ vertices where every pair of distinct vertices is connected
#flashcards/fundamentals-of-computer-science/graph-theory/special-types

What is the complete bipartite graph $K_{m,n}$?::$K_{m,n} = ([m] \cup [n], \{(i,j) : i \in [m], j \in [n]\})$ - a bipartite graph where every vertex in one part connects to every vertex in the other part
#flashcards/fundamentals-of-computer-science/graph-theory/special-types

How would you describe complete graphs in simple terms?::Every pair of distinct vertices is connected by exactly one edge
#flashcards/fundamentals-of-computer-science/graph-theory/special-types

How would you describe complete bipartite graphs in simple terms?::A bipartite graph where all vertices are connected to all vertices they can connect to (across the partition)
#flashcards/fundamentals-of-computer-science/graph-theory/special-types