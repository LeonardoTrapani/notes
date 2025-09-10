## Open and Closed Set Theorems

### Fundamental Relationship

**Theorem**: $A \subseteq \mathbb{R}$ is open $\Leftrightarrow A^c$ is closed

**Theorem**: $A \subseteq \mathbb{R}$ is closed $\Leftrightarrow A$ contains all its accumulation points

### Properties of Open Sets

**Theorem**: The following properties hold for open sets:

**(i)** The intersection of a **finite** number of open sets is open

**(ii)** The union of a **finite/infinite** number of open sets is open

**Important Note**: Property (i) is **not valid** for an infinite number of open sets.

**Counterexample**: Consider $A_m = (-\frac{1}{m}, \frac{1}{m})$ for $m \in \mathbb{N}$:
$$\bigcap_{m} A_m = \{0\} \text{ (closed)}$$

### Properties of Closed Sets

**Theorem**: The following properties hold for closed sets:

**(iii)** The intersection of a **finite/infinite** number of closed sets is closed

**(iv)** The union of a **finite** number of closed sets is closed

**Important Note**: Property (iv) is **not valid** for an infinite number of closed sets.

**Counterexample**: Consider $A_m = [0, 1 - \frac{1}{m}]$ for $m \in \mathbb{N}$:
$$\bigcup_{m} A_m = [0, 1) \text{ (not closed)}$$

### Special Sets

Consider $\mathbb{R} = (-\infty, +\infty)$:
- All its points are interior points, so $\mathbb{R}$ is open
- The boundary of $\mathbb{R}$ is $\emptyset$, and $\emptyset \subseteq \mathbb{R}$, so $\mathbb{R}$ is closed

Therefore: $\emptyset = \mathbb{R}^c$ is open

The boundary of $\mathbb{R}$ is $\emptyset$, and $\emptyset \subseteq \mathbb{R}$, so $\mathbb{R}$ contains its boundary, hence $\mathbb{R}$ is closed.

Therefore: $\emptyset = \mathbb{R}^c$ is open

### Example Analysis

For $A = \{\frac{1}{m+1} : m \in \mathbb{N}\} = \{1, \frac{1}{2}, \frac{1}{3}, \frac{1}{4}, \ldots\}$:

- Set $A$ is **not open** (the point $\frac{1}{2}$ is not interior)
- The points of $A$ are all isolated, but they tend to get "very close" to zero
- The boundary of $A$ is: $\partial A = A \cup \{0\}$
- Since $\partial A \not\subseteq A$ (because $0 \notin A$), then $A$ is **not closed**

---
#### Sources
[[Lecture_3.pdf]]
#### Class
[[Math and Statistics]]