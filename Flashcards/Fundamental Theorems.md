# Fundamental Theorems Flashcards

Source: [[Graph Theory Index]]
Tags: #flashcards/fundamentals-of-computer-science/graph-theory/theorems

## Handshaking Lemma
State the Handshaking Lemma::$\sum_{v \in V} d_G(v) = 2|E|$ - the sum of all vertex degrees equals twice the number of edges
#flashcards/fundamentals-of-computer-science/graph-theory/theorems

How is the Handshaking Lemma proved using the incidence matrix?::Row $v$ has $d_G(v)$ ones, so total ones = $\sum_{v \in V} d_G(v)$. Column $e$ has exactly 2 ones, so total ones = $2|E|$. Since both count the same thing, they're equal
#flashcards/fundamentals-of-computer-science/graph-theory/theorems

Explain the Handshaking Lemma in simple terms::Each edge contributes 1 to the degree of each of its two endpoints, so counting all degrees counts each edge exactly twice
#flashcards/fundamentals-of-computer-science/graph-theory/theorems

Why is it called the "Handshaking" Lemma?::In a room where people shake hands, the total number of handshakes (each person counts handshakes made) equals twice the number of actual handshakes, since each handshake involves two people
#flashcards/fundamentals-of-computer-science/graph-theory/theorems

## Corollary - Odd Degree Vertices  
State the corollary about odd degree vertices::In any graph, the number of vertices of odd degree is even
#flashcards/fundamentals-of-computer-science/graph-theory/theorems

How is the odd degree vertices corollary proved?::Let $ODD$ = odd degree vertices, $EVEN$ = even degree vertices. Then $\sum_{v \in ODD} d(v) = 2|E| - \sum_{v \in EVEN} d(v)$. Since the right side is even, the left side must be even, so $|ODD|$ is even
#flashcards/fundamentals-of-computer-science/graph-theory/theorems

Why must the number of odd-degree vertices be even?::The sum of all degrees is even (Handshaking Lemma). The sum of even degrees is even. So the sum of odd degrees must be even, which requires an even number of odd terms
#flashcards/fundamentals-of-computer-science/graph-theory/theorems

Explain the odd degree vertices result in simple terms::You can't have an odd number of people who each shook hands an odd number of times, because the total handshakes would be odd, but each handshake involves exactly two people
#flashcards/fundamentals-of-computer-science/graph-theory/theorems