# Graph Theory - Advanced Properties Flashcards

Source: [[Graph Theory Index]]
Tags: #flashcards/computer-science/graph-theory/advanced-properties

## Isomorphism
When are two graphs $G_1 = (V_1, E_1)$ and $G_2 = (V_2, E_2)$ isomorphic?::When there exists a bijection $f : V_1 \to V_2$ such that $(v,w) \in E_1 \leftrightarrow (f(v), f(w)) \in E_2$
Source: [[Isomorphism]]
#flashcards/computer-science/graph-theory/advanced-properties

What does it mean for graphs to be isomorphic in simple terms?::They have the same structural properties despite potentially having different vertex labels - they're "the same graph" up to relabeling
Source: [[Isomorphism]]
#flashcards/computer-science/graph-theory/advanced-properties

What must be preserved in a graph isomorphism?::The edge relationship - vertices are adjacent in $G_1$ if and only if their images are adjacent in $G_2$
Source: [[Isomorphism]]
#flashcards/computer-science/graph-theory/advanced-properties

## Perfect Matching
What is a perfect matching in a bipartite graph?::A set of edges that enables every vertex to be paired with exactly one other vertex
Source: [[Perfect Matching]]
#flashcards/computer-science/graph-theory/advanced-properties

Do all bipartite graphs have perfect matchings?::No, not all bipartite graphs have perfect matchings
Source: [[Perfect Matching]]
#flashcards/computer-science/graph-theory/advanced-properties

## Vertex Colouring
What is a proper vertex colouring?::An assignment of colours to vertices such that no two adjacent vertices have the same colour
Source: [[Chromatic Number]]
#flashcards/computer-science/graph-theory/advanced-properties

What is the chromatic number $\chi(G)$?::The minimum number of colours required for a proper vertex colouring of graph $G$
Source: [[Chromatic Number]]
#flashcards/computer-science/graph-theory/advanced-properties

Give a real-world application of vertex colouring::Exam scheduling: vertices represent exams, edges represent conflicts (students taking both exams), and $\chi(G)$ is the minimum number of time periods needed so no student has conflicting exams
Source: [[Chromatic Number]]
#flashcards/computer-science/graph-theory/advanced-properties

Name three applications of vertex colouring::Exam scheduling, register allocation in compilers, map coloring problems
Source: [[Chromatic Number]]
#flashcards/computer-science/graph-theory/advanced-properties