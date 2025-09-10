Source: [[Lecture_2.pdf]] and [[Lecture_3.pdf]]

#flashcards/math/analysis/sets #flashcards/math/analysis/topology

## Set Theory and Real Analysis Fundamentals

What is the infimum of a set A ⊆ ℝ?
?
The infimum (inf A) is the greatest lower bound of set A. It's the largest number that is less than or equal to all elements in A.

What is the supremum of a set A ⊆ ℝ?
?
The supremum (sup A) is the least upper bound of set A. It's the smallest number that is greater than or equal to all elements in A.

When does a set A have a maximum?
?
A set A has a maximum when sup A ∈ A (the supremum belongs to the set). Then max A = sup A.

When does a set A have a minimum?
?
A set A has a minimum when inf A ∈ A (the infimum belongs to the set). Then min A = inf A.

For the set A = {1/(m+1), m ∈ ℕ} = {1, 1/2, 1/3, 1/4, ...}, what are sup A, inf A, max A, and min A?
?
- sup A = max A = 1 (achieved when m = 1)
- inf A = 0 (greatest lower bound, but 0 ∉ A)
- min A does not exist (since inf A ∉ A)

What is the absolute value |x| of x ∈ ℝ geometrically?
?
|x| is the distance from 0 of x ∈ ℝ. More generally, d(x,0) = |x| for all x ∈ ℝ.

How is distance defined between two points x, y ∈ ℝ?
?
The distance between x and y is defined as d(x,y) = |y - x| = |x - y|.

What is the neighborhood N_τ(x₀) of a point x₀ ∈ ℝ with radius τ > 0?
?
N_τ(x₀) = {x ∈ ℝ : d(x, x₀) < τ} = {x ∈ ℝ : |x - x₀| < τ} = (x₀ - τ, x₀ + τ)

What does d(x, x₀) < τ mean in terms of inequalities?
?
d(x, x₀) < τ means |x - x₀| < τ, which is equivalent to -τ < x - x₀ < τ, or x₀ - τ < x < x₀ + τ.

Define an interior point of a set A ⊆ ℝ.
?
x₀ is an interior point of A if there exists N_τ(x₀) such that N_τ(x₀) ⊆ A.

Define an exterior point of a set A ⊆ ℝ.
?
x₀ is an exterior point of A if there exists N_τ(x₀) such that N_τ(x₀) ⊆ Aᶜ (the complement of A).

Define a boundary point of a set A ⊆ ℝ.
?
x₀ is a boundary point of A if for all N_τ(x₀) we have N_τ(x₀) ∩ A ≠ ∅ and N_τ(x₀) ∩ Aᶜ ≠ ∅.

Define an accumulation point of a set A ⊆ ℝ.
?
x₀ is an accumulation point of A if for all N_τ(x₀) we have A ∩ N_τ(x₀)\{x₀} ≠ ∅ (the neighborhood of x₀ without x₀ contains points of A).

What is an isolated point of a set A ⊆ ℝ?
?
x₀ is an isolated point of A if there exists N_τ(x₀) such that N_τ(x₀) ∩ A = {x₀}.

Define neighborhood of +∞.
?
N(+∞) = (a, +∞) with a ∈ ℝ. Examples: (-100, +∞), (3, +∞), (-20, +∞).

Define neighborhood of -∞.
?
N(-∞) = (-∞, a) with a ∈ ℝ. Examples: (-∞, -50), (-∞, 0), (-∞, 8).

Define an open set in ℝ.
?
A set A ⊆ ℝ is open when all the points of A are interior points (int A = A).

Define a closed set in ℝ.
?
A set A ⊆ ℝ is closed when it contains all its boundary points (∂A ⊆ A).

What is the relationship between open and closed sets?
?
A ⊆ ℝ is open ⟺ Aᶜ is closed.

A ⊆ ℝ is closed ⟺ A contains all its accumulation points.
?
True. This is an equivalent definition of a closed set.

Which sets are both open and closed in ℝ?
?
ℝ and ∅ are open and closed at the same time. These are the only two exceptions.

State the theorem about intersection of open sets.
?
The intersection of a finite number of open sets is open.

State the theorem about union of open sets.
?
The union of a finite/infinite number of open sets is open.

State the theorem about intersection of closed sets.
?
The intersection of a finite/infinite number of closed sets is closed.

State the theorem about union of closed sets.
?
The union of a finite number of closed sets is closed.

Why is the intersection of an infinite number of open sets not necessarily open?
?
Counterexample: A_m = (-1/m, 1/m), then ⋂_m A_m = {0}, which is closed, not open.

Why is the union of an infinite number of closed sets not necessarily closed?
?
Counterexample: A_m = [0, 1-1/m], then ⋃_m A_m = [0, 1), which is not closed.

Define a compact set in ℝ.
?
A set A ⊆ ℝ is compact when A is closed and bounded.

Give examples of compact sets.
?
- A = [-10, 5] is compact
- B = [-10, 0] ∪ [3, 5] is compact  
- C = [-20, -10] ∪ {50} is compact
- D = {1} ∪ {3} ∪ {50} is compact

For the set A = (-∞, 2) ∪ [5, 7] ∪ (10, 30] ∪ {35}, classify the points 0, 0, 9, 2, 2, and 35.
?
- 0 is an interior point of A
- 0 is an accumulation point of A  
- 9 is an exterior point of A
- 2 is a boundary point of A
- 2 is an accumulation point of A
- 35 is an isolated point

Given the set A = (-∞, 2) ∪ [5, 7] ∪ (10, 30] ∪ {35}, what are int A, ∂A, and A'?
?
- int A = (-∞, 2) ∪ (5, 7) ∪ (10, 30)
- ∂A = {2, 5, 7, 10, 30, 35}  
- A' = (-∞, 2] ∪ [5, 7] ∪ [10, 30]

What does the max function max(x, -x) choose between x and -x?
?
max(x, -x) chooses the greatest between x and -x. If x ≥ -x, it chooses x; if x < -x, it chooses -x.

What does the min function min(x, -x) choose between x and -x?
?
min(x, -x) chooses the smallest between x and -x.

For a collection of intervals A_m = (-1/m, 1/m), what is the intersection ⋂_m A_m?
?
When A₁ ⊃ A₂ ⊃ A₃ ⊃ ..., we have that the unique element in common (the intersection) is 0. Then A = {0}.

What are the key properties that distinguish interior, exterior, boundary, and accumulation points?
?
- Interior: neighborhood entirely in A
- Exterior: neighborhood entirely in Aᶜ  
- Boundary: every neighborhood intersects both A and Aᶜ
- Accumulation: every neighborhood contains other points of A
- Isolated: neighborhood intersects A only at the point itself