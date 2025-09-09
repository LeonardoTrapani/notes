#flashcards [[Graph Theory Index]]
# Graph Theory - Basic Definitions Flashcards

## Simple Graph Definition
What is a simple graph?::A simple graph G = (V, E) where V = {vertices} and E = {edges}. Each edge connects exactly two vertices with no loops or multiple edges between the same pair of vertices.

A graph with no {{c1::loops}} or {{c1::multiple edges}} between the same pair of vertices is called a {{c2::simple graph}}.

## Vertex Degrees
What does d_G(v) represent?::The degree of vertex v in graph G, which is the number of edges incident with v.

The {{c1::minimum degree}} of a graph G is denoted as {{c2::δ(G) = min_v d_G(v)}}.

The {{c1::maximum degree}} of a graph G is denoted as {{c2::Δ(G) = max_v d_G(v)}}.

## Subgraphs
When is G' = (V', E') a subgraph of G = (V, E)?::When V' ⊆ V and E' ⊆ E.

A subgraph G' is called a {{c1::spanning subgraph}} if {{c2::V' = V}} (it contains all vertices of the original graph).

What is the difference between a subgraph and an induced subgraph?::A subgraph can have any subset of edges from the original graph, while an induced subgraph must contain ALL edges between the chosen vertices that exist in the original graph.

## Induced Subgraphs
If V' ⊆ V, what is G[V']?::G[V'] = (V', {(u,v) ∈ E : u,v ∈ V'}), the subgraph of G induced by V'.

For edge-induced subgraph G[E₁] where E₁ ⊆ E, what is V₁?::V₁ = {v ∈ V : ∃e ∈ E₁ such that v ∈ e} - all vertices that are endpoints of edges in E₁.

## Isomorphism
When are two graphs G₁ and G₂ isomorphic?::When there exists a bijection f : V₁ → V₂ such that (v,w) ∈ E₁ ↔ (f(v), f(w)) ∈ E₂.

True or False: Isomorphic graphs have the same structural properties despite potentially having different vertex labels.::True.

What does it mean for graphs to be structurally equivalent?::They are {{c1::isomorphic}} - there exists a bijection between their vertices that preserves adjacency relationships.