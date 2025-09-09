#flashcards [[Graph Theory Index]]
# Graph Theory - Special Graph Types Flashcards

## Complete Graphs
What is K_n?::K_n = ([n], {(i,j) : 1 ≤ i < j ≤ n}) is the complete graph on n vertices.

What is K_{m,n}?::K_{m,n} = ([m] ∪ [n], {(i,j) : i ∈ [m], j ∈ [n]}) is the complete bipartite graph on m + n vertices.

In a complete graph, how are the vertices connected?::Every pair of distinct vertices is connected by exactly one edge.

How many edges does K_n have?::{{c1::n(n-1)/2}} edges, since every pair of vertices is connected exactly once.

## Bipartite Graphs
What defines a bipartite graph?::G is bipartite if V = X ∪ Y where X and Y are disjoint and every edge is of the form (x,y) where x ∈ X and y ∈ Y.

A bipartite graph has vertices that can be divided into {{c1::two disjoint sets}} such that {{c2::no two vertices within the same set are adjacent}}.

True or False: In a bipartite graph, all edges connect vertices from different sets.::True.
<!--SR:!2025-09-13,4,270-->

What is a complete bipartite graph K_{m,n}?::A bipartite graph where every vertex in the first set of size m is connected to every vertex in the second set of size n.

## Perfect Matching
What is a perfect matching in a bipartite graph?::A set of edges that enables every vertex to be paired with exactly one other vertex.

True or False: All bipartite graphs have perfect matchings.::False. Not all bipartite graphs have perfect matchings.

For a perfect matching to exist in a bipartite graph with sets X and Y, what must be true about |X| and |Y|?::{{c1::|X| = |Y|}} - the sets must have equal size.