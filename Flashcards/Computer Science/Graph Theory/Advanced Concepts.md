#flashcards [[Graph Theory Index]]
# Graph Theory - Advanced Concepts Flashcards

## Isomorphism Detection
What are some properties that isomorphic graphs must share?::{{c1::Same number of vertices}}, {{c2::same number of edges}}, {{c3::same degree sequence}}.

True or False: If two graphs have the same degree sequence, they are isomorphic.::False. Same degree sequence is necessary but not sufficient for isomorphism.

Two graphs G₁ and G₂ are isomorphic if there exists a {{c1::bijection}} f: V₁ → V₂ that {{c2::preserves adjacency}}.

## Subgraph vs Induced Subgraph
Given graph G with vertices {1,2,3,4} and edges {(1,2), (1,3), (2,3), (3,4)}, what is G[{1,2,3}]?::The induced subgraph with vertices {1,2,3} and edges {(1,2), (1,3), (2,3)} - all edges between the chosen vertices.

What's the difference between selecting vertices {1,2,3} and their edges vs. taking the induced subgraph G[{1,2,3}]?::A regular subgraph can omit some edges between chosen vertices, while {{c1::induced subgraph must include ALL edges}} between the chosen vertices.

## Perfect Matching Conditions
In a bipartite graph G = (X ∪ Y, E), what is a necessary condition for a perfect matching?::{{c1::|X| = |Y|}} - both parts must have the same size.

True or False: |X| = |Y| is sufficient for a perfect matching in any bipartite graph.::False. It's necessary but not sufficient. The graph also needs sufficient connectivity.

## Matrix Analysis
If the adjacency matrix A satisfies A² = A, what can you conclude about the graph?::The graph has no {{c1::paths of length 2}}, meaning it has no triangles and each connected component is either an isolated vertex or an edge.

In the incidence matrix, what does the sum of all entries equal?::{{c1::2|E|}}, because each edge contributes exactly 2 to the total count.

## Graph Construction
How many different labeled complete graphs K_n are there on n vertices?::{{c1::1}}, because in a complete graph every pair of vertices is connected, so labeling doesn't create different structures.

How many edges does the complete bipartite graph K_{m,n} have?::{{c1::mn}} edges, because every vertex in the first set connects to every vertex in the second set.

## Chromatic Number Bounds
For any graph G, χ(G) ≥ ?::χ(G) ≥ {{c1::ω(G)}} where ω(G) is the size of the largest clique.

What is ω(G)?::The {{c1::clique number}} - the size of the largest complete subgraph in G.

For any graph G, what's the relationship between χ(G) and the independence number α(G)?::χ(G) · α(G) ≥ {{c1::|V|}}, where α(G) is the size of the largest independent set.

## Special Cases
What is χ(G) for a tree on n ≥ 2 vertices?::{{c1::2}}, because trees are bipartite (no odd cycles).

What is χ(G) for a cycle of length n?::{{c1::2}} if n is even, {{c2::3}} if n is odd.

In a graph where every vertex has degree 2, what can you say about the structure?::The graph consists of {{c1::disjoint cycles}}.