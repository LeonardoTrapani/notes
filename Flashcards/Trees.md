# Trees Flashcards

Source: [[Graph Theory Index]]
Tags: #flashcards/fundamentals-of-computer-science/graph-theory/trees

## Trees Definition
What is a tree?::A graph that is (a) connected and (b) acyclic (has no cycles)
#flashcards/fundamentals-of-computer-science/graph-theory/trees

What are the key intuitive properties of trees?::Every pair of vertices has exactly one path between them; removing any edge disconnects the tree; adding any edge creates exactly one cycle
#flashcards/fundamentals-of-computer-science/graph-theory/trees

How do trees relate to connectivity?::Trees are minimal connected graphs - they have exactly enough edges to maintain connectivity without creating cycles
#flashcards/fundamentals-of-computer-science/graph-theory/trees

## Tree Properties
If a tree $T$ has $n$ vertices, how many edges does it have?::$n - 1$ edges
#flashcards/fundamentals-of-computer-science/graph-theory/trees

If a tree has $n \geq 2$ vertices, what can you say about vertices of degree 1?::It has at least 2 vertices of degree 1 (leaf vertices)
#flashcards/fundamentals-of-computer-science/graph-theory/trees

Why must trees have at least 2 leaf vertices? (For $n \geq 2$)::Let $s$ = number of degree-1 vertices. By Handshaking Lemma: $2(n-1) = \sum d(v) \geq 2(n-s) + s$, so $2n - 2 \geq 2n - s$, giving $s \geq 2$
#flashcards/fundamentals-of-computer-science/graph-theory/trees

Why do trees have exactly $n-1$ edges?::Trees are minimally connected - they need at least $n-1$ edges for connectivity, and having more would create cycles
#flashcards/fundamentals-of-computer-science/graph-theory/trees

## Tree Equivalence
For a graph with $n$ vertices and $n-1$ edges, what three conditions are equivalent?::(a) $G$ is connected, (b) $G$ is acyclic, (c) $G$ is a tree
#flashcards/fundamentals-of-computer-science/graph-theory/trees

What is the significance of the Tree Equivalence theorem?::With exactly $n-1$ edges, any one property (connected, acyclic, or tree) implies the others - you only need to check one condition
#flashcards/fundamentals-of-computer-science/graph-theory/trees

What does the Tree Equivalence theorem tell us about minimal connectivity?::Trees are precisely the minimal connected graphs - they achieve connectivity with the minimum possible number of edges
#flashcards/fundamentals-of-computer-science/graph-theory/trees