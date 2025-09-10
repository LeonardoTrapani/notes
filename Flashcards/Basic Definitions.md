# Basic Definitions Flashcards

Source: [[Graph Theory Index]]
Tags: #flashcards/fundamentals-of-computer-science/graph-theory/basic-definitions

## Simple Graph
What are the two components of a simple graph $G$?::$G = (V, E)$ where $V = \{vertices\}$ and $E = \{edges\}$
#flashcards/fundamentals-of-computer-science/graph-theory/basic-definitions

## Vertex Degrees
What is the notation for the degree of vertex $v$ in graph $G$?::$d_G(v) =$ number of edges incident with $v$
#flashcards/fundamentals-of-computer-science/graph-theory/basic-definitions

What is the notation for minimum degree in graph $G$?::$\delta(G) = \min_v d_G(v)$
#flashcards/fundamentals-of-computer-science/graph-theory/basic-definitions

What is the notation for maximum degree in graph $G$?::$\Delta(G) = \max_v d_G(v)$
#flashcards/fundamentals-of-computer-science/graph-theory/basic-definitions

## Subgraphs
When is $G' = (V', E')$ a subgraph of $G = (V, E)$?::When $V' \subseteq V$ and $E' \subseteq E$
#flashcards/fundamentals-of-computer-science/graph-theory/basic-definitions

What is a spanning subgraph?::A subgraph $G'$ where $V' = V$ (all vertices are the same, but different edges)
#flashcards/fundamentals-of-computer-science/graph-theory/basic-definitions

## Induced Subgraph
For vertex set $V' \subseteq V$, what is the induced subgraph $G[V']$?::$G[V'] = (V', \{(u,v) \in E : u,v \in V'\})$ - includes all edges between vertices in $V'$
#flashcards/fundamentals-of-computer-science/graph-theory/basic-definitions

What does inducing a subgraph by a vertex set mean in simple terms?::Select a subset of vertices, and include all edges that connect vertices within that subset
#flashcards/fundamentals-of-computer-science/graph-theory/basic-definitions

Given edge set $E_1 \subseteq E$, what is the induced subgraph $G[E_1]$?::$G[E_1] = (V_1, E_1)$ where $V_1 = \{v \in V : \exists e \in E_1 \text{ such that } v \in e\}$
#flashcards/fundamentals-of-computer-science/graph-theory/basic-definitions

What does inducing a subgraph by an edge set mean in simple terms?::Given a subset of edges, take all vertices that are connected by those edges in the original graph
#flashcards/fundamentals-of-computer-science/graph-theory/basic-definitions