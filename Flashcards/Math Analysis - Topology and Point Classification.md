# Math Analysis - Topology and Point Classification

Source: [[Notes/Real Number Theory Index]] - Neighborhoods and Point Types in Real Analysis

Tags: #flashcards/math/topology

---

## Neighborhoods in Real Numbers

Define a neighborhood of $x_0$ with radius $r$::$N_r(x_0) = \{x \in \mathbb{R} : d(x, x_0) < r\} = \{x \in \mathbb{R} : |x - x_0| < r\}$
Source: [[Neighborhoods in Real Numbers]]

What is the interval representation of $N_r(x_0)$?::$N_r(x_0) = (x_0 - r, x_0 + r)$ (an open interval with extremes excluded)
Source: [[Neighborhoods in Real Numbers]]

Define right neighborhood of $x_0$::$N_r^+(x_0) = [x_0, x_0 + r)$ (includes $x_0$ but excludes $x_0 + r$)
Source: [[Neighborhoods in Real Numbers]]

Define left neighborhood of $x_0$::$N_r^-(x_0) = (x_0 - r, x_0]$ (excludes $x_0 - r$ but includes $x_0$)
Source: [[Neighborhoods in Real Numbers]]

Are right and left neighborhoods true neighborhoods in the strict sense?::No, despite their names, they are **not neighborhoods** in the strict sense because extremes are not excluded and $x_0 \in N_r^+(x_0)$ and $x_0 \in N_r^-(x_0)$
Source: [[Neighborhoods in Real Numbers]]

Define neighborhood of $+\infty$::$N(+\infty) = (a, +\infty)$ with $a \in \mathbb{R}$ (e.g., $(-100, +\infty)$, $(3, +\infty)$)
Source: [[Neighborhoods in Real Numbers]]

Define neighborhood of $-\infty$::$N(-\infty) = (-\infty, a)$ with $a \in \mathbb{R}$ (e.g., $(-\infty, -50)$, $(-\infty, 0)$)
Source: [[Neighborhoods in Real Numbers]]

---

## Types of Points in Sets

Define interior point of set $A$::$x_0$ is an interior point if there exists $N_r(x_0)$ such that $N_r(x_0) \subseteq A$ (the point has a full neighborhood contained within the set)
Source: [[Interior Points]]

What is the notation for the set of interior points of $A$?::$\text{int } A$
Source: [[Interior Points]]

Define exterior point of set $A$::$x_0$ is an exterior point if there exists $N_r(x_0)$ such that $N_r(x_0) \subseteq A^c$ (the point has a full neighborhood in the complement of the set)
Source: [[Exterior Points]]

What is the notation for the set of exterior points of $A$?::$\text{int } A^c$
Source: [[Exterior Points]]

Define boundary point of set $A$::$x_0$ is a boundary point if for every $N_r(x_0)$ we have $N_r(x_0) \cap A \neq \emptyset$ AND $N_r(x_0) \cap A^c \neq \emptyset$ (every neighborhood intersects both the set and its complement)
Source: [[Boundary Points]]

What is the notation for the set of boundary points of $A$?::$\partial A$
Source: [[Boundary Points]]

Define accumulation point of set $A$::$x_0$ is an accumulation point if for every $N_r(x_0)$ we have $A \cap N_r(x_0) \setminus \{x_0\} \neq \emptyset$ (every neighborhood contains points of $A$ other than $x_0$ itself)
Source: [[Accumulation Points]]

What does $N_r(x_0) \setminus \{x_0\}$ represent?::The neighborhood of $x_0$ without $x_0$ itself: $(x_0 - r, x_0) \cup (x_0, x_0 + r)$
Source: [[Accumulation Points]]

Define isolated point of set $A$::$x_0$ is an isolated point if there exists $N_r(x_0)$ such that $N_r(x_0) \cap A = \{x_0\}$ (a neighborhood containing only $x_0$ from set $A$)
Source: [[Isolated Points]]

What is the relationship between isolated points and other point types?::Isolated points are a particular case of boundary points that are not accumulation points
Source: [[Isolated Points]]

---

## Point Classification Examples

For set $A = (-\infty, 2) \cup [5, 7] \cup (10, 30) \cup \{35\}$, classify point 0::$0$ is both an interior point and an accumulation point of $A$ (has full neighborhood in $(-\infty, 2)$)
Source: [[Interior Points]]

For set $A = (-\infty, 2) \cup [5, 7] \cup (10, 30) \cup \{35\}$, classify point 9::$9$ is an exterior point of $A$
Source: [[Exterior Points]]

For set $A = (-\infty, 2) \cup [5, 7] \cup (10, 30) \cup \{35\}$, classify point 2::$2$ is both a boundary point and an accumulation point of $A$
Source: [[Boundary Points]]

For set $A = (-\infty, 2) \cup [5, 7] \cup (10, 30) \cup \{35\}$, classify point 35::$35$ is an isolated point
Source: [[Isolated Points]]

---

## Key Relationships Between Point Types

What is the relationship between interior points and accumulation points?::$x_0 \in \text{int } A \Rightarrow x_0$ is an accumulation point of $A$
Source: [[Interior Points]]

What is the relationship between boundary points (not isolated) and accumulation points?::$x_0 \in \partial A \Rightarrow x_0$ is an accumulation point of $A$ (for non-isolated boundary points)
Source: [[Boundary Points]]