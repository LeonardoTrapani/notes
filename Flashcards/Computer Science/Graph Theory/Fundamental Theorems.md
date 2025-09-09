#flashcards [[Graph Theory Index]]
# Graph Theory - Fundamental Theorems Flashcards

## Handshaking Lemma
State the Handshaking Lemma::$$\sum_{v \in V} d_G(v) = 2|E|$$

What does the Handshaking Lemma say in words?::The sum of all vertex degrees equals twice the number of edges.

Why does the sum of degrees equal 2|E|?::Because each edge contributes {{c1::2}} to the total degree count (once for each of its {{c2::endpoints}}).

## Proof of Handshaking Lemma
How is the Handshaking Lemma proven using the incidence matrix?::Consider the incidence matrix M. Row v has d_G(v) 1's, so total 1's = Σd_G(v). Column e has exactly 2 1's, so total 1's = 2|E|. Therefore Σd_G(v) = 2|E|.

In the incidence matrix proof, why does each column have exactly 2 ones?::Because each {{c1::edge}} connects exactly {{c2::two vertices}}.

## Corollary - Odd Degree Vertices
State the corollary about odd degree vertices::In any graph, the number of vertices of odd degree is even.

Why must the number of odd-degree vertices be even?::Let ODD = {odd degree vertices} and EVEN = V \ ODD. Then Σ_{v∈ODD} d(v) = 2|E| - Σ_{v∈EVEN} d(v). Since the right side is even, |ODD| must be even.

Complete the equation: $$\sum_{v \in ODD} d(v) = ?$$::$$\sum_{v \in ODD} d(v) = 2|E| - \sum_{v \in EVEN} d(v)$$

True or False: A graph can have exactly 3 vertices of odd degree.::False. The number of odd-degree vertices must be even.

## Applications of the Handshaking Lemma
If a graph has 10 vertices each of degree 3, how many edges does it have?::{{c1::15}} edges, because Σd(v) = 30, so |E| = 30/2 = 15.

In a graph with n vertices, what's the maximum possible sum of degrees?::{{c1::n(n-1)}} when the graph is complete, achieved by K_n.