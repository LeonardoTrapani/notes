## Types of Points in Sets

For a set $A \subseteq \mathbb{R}$ and a point $x_0 \in \mathbb{R}$, we classify points based on their relationship with neighborhoods.

### Interior Points

$x_0$ is an **interior point** of $A$ if there exists $N_r(x_0)$ such that $N_r(x_0) \subseteq A$.

- The point has a full neighborhood contained within the set
- **Notation**: The set of interior points is $\text{int } A$

### Exterior Points  

$x_0$ is an **exterior point** of $A$ if there exists $N_r(x_0)$ such that $N_r(x_0) \subseteq A^c$.

- The point has a full neighborhood contained in the complement of the set
- **Notation**: The set of exterior points is $\text{int } A^c$

### Boundary Points

$x_0$ is a **boundary point** of $A$ if for every $N_r(x_0)$ we have:
- $N_r(x_0) \cap A \neq \emptyset$ AND  
- $N_r(x_0) \cap A^c \neq \emptyset$

- Every neighborhood intersects both the set and its complement
- **Notation**: The set of boundary points is $\partial A$

### Accumulation Points

$x_0$ is an **accumulation point** of $A$ if for every $N_r(x_0)$ we have:
$$A \cap N_r(x_0) \setminus \{x_0\} \neq \emptyset$$

- Every neighborhood contains points of $A$ other than $x_0$ itself
- **Note**: The neighborhood of $x_0$ without $x_0$ is $(x_0 - r, x_0) \cup (x_0, x_0 + r)$

### Isolated Points

$x_0$ is an **isolated point** of $A$ if there exists $N_r(x_0)$ such that:
$$N_r(x_0) \cap A = \{x_0\}$$

- There exists a neighborhood containing only $x_0$ from the set $A$
- Isolated points are a particular case of boundary points that are not accumulation points

### Example Analysis

For $A = (-\infty, 2) \cup [5, 7] \cup (10, 30) \cup \{35\}$:

- $0$ is an **interior point** of $A$ (has full neighborhood in $(-\infty, 2)$)
- $0$ is an **accumulation point** of $A$  
- $9$ is an **exterior point** of $A$
- $2$ is a **boundary point** of $A$
- $2$ is an **accumulation point** of $A$  
- $35$ is an **isolated point**

### Key Relationships

- **Interior points**: $x_0 \in \text{int } A \Rightarrow x_0$ is accumulation point of $A$
- **Boundary points (not isolated)**: $x_0 \in \partial A \Rightarrow x_0$ is accumulation point of $A$

---
#### Sources
[[Lecture_2.pdf]]
#### Class
[[Math and Statistics]]