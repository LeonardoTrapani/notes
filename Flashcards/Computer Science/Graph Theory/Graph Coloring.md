#flashcards [[Graph Theory Index]]
# Graph Theory - Graph Coloring Flashcards

## Vertex Coloring
What is a proper vertex coloring?::An assignment of colors to vertices such that no two adjacent vertices have the same color.

What is the chromatic number χ(G)?::The minimum number of colors required for a proper vertex coloring of graph G.

For a proper vertex coloring, adjacent vertices must have {{c1::different colors}}.

## Chromatic Number Properties
What is χ(K_n) for a complete graph?::{{c1::n}}, because every vertex is adjacent to every other vertex, so each needs a unique color.

What is χ(G) for any bipartite graph G?::{{c1::2}}, because you can color one set with color 1 and the other set with color 2.

True or False: χ(G) ≤ Δ(G) + 1 for any graph G.::True. This is a fundamental upper bound (though not always tight).

## Applications of Graph Coloring
Describe the exam scheduling application of graph coloring::V = {exams}, (a,b) is an edge iff there is some student who needs to take both exams. χ(G) is the minimum number of periods required so that no student takes two exams simultaneously.

In the exam scheduling problem, what do vertices represent?::{{c1::Exams}}

In the exam scheduling problem, what do edges represent?::{{c1::Conflicts}} - when the same student needs to take both exams.

In the exam scheduling problem, what does the chromatic number represent?::The {{c1::minimum number of time periods}} needed to schedule all exams without conflicts.

## Other Coloring Applications
Name two other applications of graph coloring besides exam scheduling::{{c1::Register allocation in compilers}} and {{c2::map coloring problems}}.

In compiler register allocation, what do vertices and edges represent?::{{c1::Vertices = variables}}, {{c2::edges = variables that interfere}} (are live at the same time).

## Bounds on Chromatic Number
If G has maximum degree Δ(G), what's an upper bound on χ(G)?::χ(G) ≤ {{c1::Δ(G) + 1}}

For a bipartite graph, χ(G) = ?::{{c1::2}} (unless the graph has no edges, in which case χ(G) = 1).