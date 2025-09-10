# Graph Properties Flashcards

Source: [[Graph Theory Index]]
Tags: #flashcards/fundamentals-of-computer-science/graph-theory/properties

## Isomorphism
When are two graphs $G_1 = (V_1, E_1)$ and $G_2 = (V_2, E_2)$ isomorphic?::When there exists a bijection $f : V_1 \to V_2$ such that $(v,w) \in E_1 \leftrightarrow (f(v), f(w)) \in E_2$
#flashcards/fundamentals-of-computer-science/graph-theory/properties

What does it mean for graphs to be isomorphic in simple terms?::They have the same structural properties despite potentially having different vertex labels - they're "the same graph" up to relabeling
#flashcards/fundamentals-of-computer-science/graph-theory/properties

What must be preserved in a graph isomorphism?::The edge relationship - vertices are adjacent in $G_1$ if and only if their images are adjacent in $G_2$
#flashcards/fundamentals-of-computer-science/graph-theory/properties

## Perfect Matching
What is a perfect matching in a bipartite graph?::A set of edges that enables every vertex to be paired with exactly one other vertex
#flashcards/fundamentals-of-computer-science/graph-theory/properties

Do all bipartite graphs have perfect matchings?::No, not all bipartite graphs have perfect matchings
#flashcards/fundamentals-of-computer-science/graph-theory/properties

## Vertex Colouring
What is a proper vertex colouring?::An assignment of colours to vertices such that no two adjacent vertices have the same colour
#flashcards/fundamentals-of-computer-science/graph-theory/properties

What is the chromatic number $\chi(G)$?::The minimum number of colours required for a proper vertex colouring of graph $G$
#flashcards/fundamentals-of-computer-science/graph-theory/properties

Give a real-world application of vertex colouring::Exam scheduling: vertices represent exams, edges represent conflicts (students taking both exams), and $\chi(G)$ is the minimum number of time periods needed so no student has conflicting exams
#flashcards/fundamentals-of-computer-science/graph-theory/properties

Name three applications of vertex colouring:::Exam scheduling, register allocation in compilers, map coloring problems
#flashcards/fundamentals-of-computer-science/graph-theory/properties