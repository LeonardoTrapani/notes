#flashcards [[Graph Theory Index]]
# Graph Theory - Matrix Representations Flashcards

## Adjacency Matrix
What is the adjacency matrix A?::A V × V matrix where A(v,w) = 1 if v,w are adjacent, and 0 otherwise.

For simple graphs, what properties does the adjacency matrix have?::The adjacency matrix is {{c1::symmetric}} with {{c2::zeros on the diagonal}}.

$$A(v,w) = \begin{cases} ? & v,w \text{ adjacent} \\ ? & \text{otherwise} \end{cases}$$::$$A(v,w) = \begin{cases} 1 & v,w \text{ adjacent} \\ 0 & \text{otherwise} \end{cases}$$

Why does the adjacency matrix of a simple graph have zeros on the diagonal?::Because simple graphs have no {{c1::self-loops}}, so no vertex is adjacent to itself.

## Incidence Matrix
What is the incidence matrix M?::M is a V × E matrix where M(v,e) = 1 if v ∈ e, and 0 if v ∉ e.

In the incidence matrix, what do rows represent and what do columns represent?::{{c1::Rows}} correspond to {{c2::vertices}}, {{c3::columns}} correspond to {{c4::edges}}.

$$M(v,e) = \begin{cases} ? & v \in e \\ ? & v \notin e \end{cases}$$::$$M(v,e) = \begin{cases} 1 & v \in e \\ 0 & v \notin e \end{cases}$$

How many 1's appear in each column of an incidence matrix for a simple graph?::{{c1::Exactly 2}}, because each edge connects exactly two vertices.

What does the sum of entries in row v of the incidence matrix equal?::The {{c1::degree}} of vertex v, denoted {{c2::d_G(v)}}.

## Relationship Between Matrices
How can you compute the degree of a vertex from the adjacency matrix?::Sum all entries in the row (or column) corresponding to that vertex.

How can you compute the degree of a vertex from the incidence matrix?::Sum all entries in the row corresponding to that vertex.