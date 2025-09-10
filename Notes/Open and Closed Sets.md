## Open and Closed Sets

### Open Set Definition

A set $A \subseteq \mathbb{R}$ is said to be **open** when all the points of $A$ are interior points.

**Formal Definition**: $A$ is open $\Leftrightarrow \text{int } A = A$

### Closed Set Definition  

A set $A \subseteq \mathbb{R}$ is said to be **closed** when it contains all its boundary points.

**Formal Definition**: $A$ is closed $\Leftrightarrow \partial A \subseteq A$

### Key Properties

**Important Remark**: A set can be neither open nor closed, and some special sets can be both open and closed simultaneously.

The two exceptions are:
- $\mathbb{R}$ is both open and closed
- $\emptyset$ (empty set) is both open and closed

### Examples

**Open Sets**:
- $A = (-2, 5) \cup (8, +\infty)$ is open
- All points in these intervals are interior points

**Closed Sets**:
- $B = [3, +\infty)$ is closed (contains its boundary point $3$: $\partial B = \{3\} \subseteq B$)

**Neither Open nor Closed**:
- $C = (-\infty, 2) \cup [3, 5]$ is neither open nor closed
  - Point $3$ is not interior (so not open)
  - Point $2$ is boundary but $2 \notin C$ (so not closed)

### Special Cases

**The Integers**: $\mathbb{Z} = \{\ldots, -2, -1, 0, 1, 2, \ldots\}$
- Made up of isolated points
- $\partial \mathbb{Z} = \mathbb{Z}$ 
- Therefore $\mathbb{Z}$ is closed in $\mathbb{R}$

---
#### Sources
[[Lecture_3.pdf]]
#### Class
[[Math and Statistics]]