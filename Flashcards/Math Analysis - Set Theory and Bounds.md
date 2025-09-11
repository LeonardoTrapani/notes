# Math Analysis - Set Theory and Bounds

Source: [[Notes/Real Number Theory Index]] - Set Theory, Bounds, and Extrema Concepts

Tags: #flashcards/math/bounds-extrema

---

## Number System Hierarchy

What is the hierarchy of fundamental number sets?::$\mathbb{N} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R}$ (Natural numbers ⊂ Integers ⊂ Rationals ⊂ Real numbers)
<!--SR:!2025-09-14,3,250-->
Source: [[Number Sets Hierarchy]]

Define the set of natural numbers $\mathbb{N}$::$\mathbb{N} = \{0, 1, 2, ...\}$
<!--SR:!2025-09-14,3,250-->
Source: [[Number Sets Hierarchy]]

Define the set of integers $\mathbb{Z}$::$\mathbb{Z} = \{..., -2, -1, 0, 1, 2, ...\}$
<!--SR:!2025-09-14,3,250-->
Source: [[Number Sets Hierarchy]]

Define the set of rational numbers $\mathbb{Q}$::$\mathbb{Q} = \{\frac{m}{n} : m, n \in \mathbb{Z} \text{ and } n \neq 0\}$
<!--SR:!2025-09-14,3,250-->
Source: [[Number Sets Hierarchy]]

What are irrational numbers?::Numbers that cannot be expressed as rational numbers $\frac{m}{n}$
<!--SR:!2025-09-15,4,270-->
Source: [[Irrational Numbers]]

Give three examples of irrational numbers::$\sqrt{2}$, $\pi$, $\sqrt[3]{7}$
<!--SR:!2025-09-15,4,270-->
Source: [[Irrational Numbers]]

Why do we need real numbers beyond rationals?::Because irrational numbers (like $\sqrt{2}$) exist and cannot be expressed as rationals, necessitating a larger number system
<!--SR:!2025-09-15,4,270-->
Source: [[Real Numbers]]

---

## Infinity Symbols

What do the symbols $+\infty$ and $-\infty$ represent?::$+\infty$ means "so far on the right" and $-\infty$ means "so far on the left"
<!--SR:!2025-09-15,4,270-->
Source: [[Infinity Symbols]]

Are $+\infty$ and $-\infty$ real numbers?::No, they are **not** real numbers - they are symbols used for convenience
<!--SR:!2025-09-15,4,270-->
Source: [[Infinity Symbols]]

---

## Order Properties and Operations

What property do real numbers have regarding comparison?::For any $x, y \in \mathbb{R}$, we can always state whether $x > y$, $x < y$, or $x = y$ (total order)
<!--SR:!2025-09-15,4,270-->
Source: [[Order Properties]]

What are the two fundamental operations in $\mathbb{R}$?::Sum ($x + y$) and Product ($x \cdot y$) - both are closed under $\mathbb{R}$
<!--SR:!2025-09-15,4,270-->
Source: [[Operations in ℝ]]

What does "closed under $\mathbb{R}$" mean for operations?::Performing sum or product on real numbers always yields real numbers
<!--SR:!2025-09-12,1,230-->
Source: [[Operations in ℝ]]

---

## Intervals

Define an interval mathematically::$A \subseteq \mathbb{R}$ is an interval when $\forall x, y \in A$, the set $\{z \in \mathbb{R} : x \leq z \leq y\} \subseteq A$
<!--SR:!2025-09-12,1,230-->
Source: [[Intervals]]

What is the difference between $[a, b]$ and $(a, b)$?::$[a, b]$ is a closed interval (endpoints included), $(a, b)$ is an open interval (endpoints not included)
<!--SR:!2025-09-15,4,270-->
Source: [[Intervals]]

Give examples of half-infinite intervals::$[a, +\infty)$ and $(-\infty, b]$
<!--SR:!2025-09-15,4,270-->
Source: [[Intervals]]

---

## Upper and Lower Bounds

Define upper bound::A number $h \in \mathbb{R}$ such that $x \leq h$ for all $x \in A$
<!--SR:!2025-09-15,4,270-->
Source: [[Upper and Lower Bounds]]

Define lower bound::A number $k \in \mathbb{R}$ such that $x \geq k$ for all $x \in A$
<!--SR:!2025-09-14,3,250-->
Source: [[Upper and Lower Bounds]]

When is a set $A$ bounded from above?::When it has an upper bound
<!--SR:!2025-09-15,4,270-->
Source: [[Upper and Lower Bounds]]

When is a set $A$ bounded from below?::When it has a lower bound
<!--SR:!2025-09-15,4,270-->
Source: [[Upper and Lower Bounds]]

When is a set $A$ bounded?::When it has both upper and lower bounds
<!--SR:!2025-09-15,4,270-->
Source: [[Upper and Lower Bounds]]

If a set has one upper bound, how many upper bounds does it have?::Infinitely many (any number greater than the bound is also an upper bound)
<!--SR:!2025-09-14,3,250-->
Source: [[Upper and Lower Bounds]]

---

## Maximum and Minimum

Define maximum of a set $A$::A number $x^* \in A$ such that $x^* \geq x$ for all $x \in A$ (denoted $\max A$)
<!--SR:!2025-09-14,3,250-->
Source: [[Maximum and Minimum]]

Define minimum of a set $A$::A number $x^* \in A$ such that $x^* \leq x$ for all $x \in A$ (denoted $\min A$)
<!--SR:!2025-09-14,3,250-->
Source: [[Maximum and Minimum]]

What is the key difference between maximum/minimum and upper/lower bounds?::Maximum and minimum must be **elements of the set** ($x^* \in A$), while bounds don't need to be
<!--SR:!2025-09-15,4,270-->
Source: [[Maximum and Minimum]]

How many maxima can a set have?::At most one (if it exists, it's unique)
<!--SR:!2025-09-15,4,270-->
Source: [[Maximum and Minimum]]

Prove uniqueness of maximum: If $x_1, x_2 \in A$ are both maxima, then what follows?::By definition: $x_1 \geq x_2$ and $x_2 \geq x_1$, therefore $x_1 = x_2$
<!--SR:!2025-09-14,3,250-->
Source: [[Maximum and Minimum]]

---

## Supremum and Infimum

Define supremum (sup)::The minimum of the upper bounds of $A$ (least upper bound)
<!--SR:!2025-09-15,4,270-->
Source: [[Infimum and Supremum]]

Define infimum (inf)::The maximum of the lower bounds of $A$ (greatest lower bound)
<!--SR:!2025-09-14,3,250-->
Source: [[Infimum and Supremum]]

What is the relationship between supremum and maximum?::If $\max A$ exists, then $\sup A = \max A$; but $\sup A$ can exist even when $\max A$ doesn't
<!--SR:!2025-09-15,4,270-->
Source: [[Infimum and Supremum]]

What is the relationship between infimum and minimum?::If $\min A$ exists, then $\inf A = \min A$; but $\inf A$ can exist even when $\min A$ doesn't
<!--SR:!2025-09-15,4,270-->
Source: [[Infimum and Supremum]]

Why are supremum and infimum important?::They provide a way to characterize bounds when maximum and minimum may not exist within the set itself
<!--SR:!2025-09-15,4,270-->
Source: [[Infimum and Supremum]]