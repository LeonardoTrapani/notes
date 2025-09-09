#flashcards [[Graph Theory Index]]
# Graph Theory - Problem Solving Flashcards

## Degree Calculations
In a graph with 8 vertices where 3 have degree 2, 3 have degree 4, and 2 have degree 5, how many edges are there?::{{c1::13}} edges. Sum of degrees = 3(2) + 3(4) + 2(5) = 6 + 12 + 10 = 28. Number of edges = 28/2 = 14. Wait, let me recalculate: 28/2 = 14 edges.

If every vertex in a graph has degree 4 and there are 12 edges, how many vertices are there?::{{c1::6}} vertices. Since Σd(v) = 2|E| = 24, and each vertex has degree 4, we have 4n = 24, so n = 6.

## Matrix Properties
If an adjacency matrix has all zeros on the diagonal, what type of graph is it?::A {{c1::simple graph}} (no self-loops).

If an adjacency matrix is symmetric, what does this tell us about the graph?::The graph is {{c1::undirected}}.

In the incidence matrix of a graph with 5 vertices and 7 edges, what are the dimensions?::{{c1::5 × 7}} (vertices × edges).

## Structural Analysis
Can a simple graph on 6 vertices have exactly 3 vertices of odd degree?::{{c1::No}}, because the number of odd-degree vertices must be even.

What's the minimum number of edges needed to connect n vertices?::{{c1::n-1}} edges (forming a tree).

What's the maximum number of edges in a simple graph with n vertices?::{{c1::n(n-1)/2}} edges (complete graph K_n).

## Bipartite Graph Recognition
How can you determine if a graph is bipartite from its adjacency matrix?::Try to arrange vertices so the adjacency matrix has a {{c1::block structure}} with zeros on the diagonal blocks.

A graph is bipartite if and only if it contains no {{c1::odd-length cycles}}.

## Coloring Problems
If a graph contains a triangle (3-cycle), what's the minimum value of χ(G)?::{{c1::3}}, because the three vertices of the triangle must all have different colors.

For the complete graph K_5, what is χ(K_5)?::{{c1::5}}, because every vertex is adjacent to every other vertex.

## Applied Problems
In a social network where edges represent friendships, what would the chromatic number represent if we want to assign people to groups?::The {{c1::minimum number of groups}} needed so that {{c2::no two friends are in the same group}}.

In a map coloring problem with 4 regions where each region borders every other region, how many colors are needed?::{{c1::4}} colors, since this forms a complete graph K_4.