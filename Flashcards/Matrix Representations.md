# Matrix Representations Flashcards

Source: [[Graph Theory Index]]
Tags: #flashcards/fundamentals-of-computer-science/graph-theory/matrices

## Adjacency Matrix
What is the adjacency matrix $A$ of a graph?::A $V \times V$ matrix where $A(v,w) = \begin{cases} 1 & \text{if } v,w \text{ adjacent} \\ 0 & \text{otherwise} \end{cases}$
#flashcards/fundamentals-of-computer-science/graph-theory/matrices

What properties does the adjacency matrix have for simple graphs?::It is symmetric and has zeros on the diagonal (no self-loops)
#flashcards/fundamentals-of-computer-science/graph-theory/matrices

## Incidence Matrix
What is the incidence matrix $M$ of a graph?::A $V \times E$ matrix where $M(v,e) = \begin{cases} 1 & \text{if } v \in e \\ 0 & \text{if } v \notin e \end{cases}$
#flashcards/fundamentals-of-computer-science/graph-theory/matrices

How do you interpret the incidence matrix?::Each row corresponds to a vertex, each column to an edge. Entry is 1 if the vertex is incident to the edge, 0 otherwise
#flashcards/fundamentals-of-computer-science/graph-theory/matrices

How many 1's appear in each column of the incidence matrix?::Exactly 2 (each edge connects exactly two vertices)
#flashcards/fundamentals-of-computer-science/graph-theory/matrices

## Walks and Matrix Powers
What does $A^k(v, w)$ represent for the adjacency matrix?::The number of walks of length $k$ from vertex $v$ to vertex $w$
#flashcards/fundamentals-of-computer-science/graph-theory/matrices

State the theorem connecting matrix powers to walks::$A^k(v, w) =$ number of walks of length $k$ from $v$ to $w$ with $k$ edges
#flashcards/fundamentals-of-computer-science/graph-theory/matrices

How is the matrix power theorem proved?::By induction: $A^{k+1}(v,w) = \sum_{u \in V} A^k(v,u)A(u,w)$ - sum over all intermediate vertices $u$ of $k$-walks from $v$ to $u$ times edges from $u$ to $w$
#flashcards/fundamentals-of-computer-science/graph-theory/matrices

What is the computational significance of the matrix power theorem?::It provides a method to compute reachability and connectivity properties using linear algebra operations
#flashcards/fundamentals-of-computer-science/graph-theory/matrices