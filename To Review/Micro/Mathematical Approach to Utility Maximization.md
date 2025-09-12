## Mathematical Approach to Utility Maximization

### The Constrained Optimization Problem
An individual's constrained optimization problem can be stated mathematically as:

$$\max_{x_1,x_2} U(x_1, x_2)$$
$$\text{s.t. } p_1x_1 + p_2x_2 = m$$

Where:
- $U(x_1, x_2)$ is the [[Utility Function Definition|utility function]]
- $p_1, p_2$ are prices (given)
- $m$ is income (given)  
- $x_1, x_2$ are choice variables

### Solution Method for Well-Behaved Preferences

#### Step 1: Set Up the System
For [[Well-Behaved Preferences|preferences that satisfy the 5 axioms]], solve the system of two equations:

**Optimality condition** (tangency):
$$\frac{MU_{x_1}}{MU_{x_2}} = \frac{p_1}{p_2}$$

**Feasibility condition** (budget constraint):
$$p_1x_1 + p_2x_2 = m$$

#### Step 2: Solve for Demand Functions
Taking prices $p_1, p_2$ and income $m$ as given parameters, solve for $x_1$ and $x_2$ as functions of these parameters:

$$x_1^* = x_1(p_1, p_2, m)$$
$$x_2^* = x_2(p_1, p_2, m)$$

These are the **[[Deriving Demand Functions Overview|Marshallian demand functions]]**.

### Special Cases

#### Non-Differentiable Utility Functions
For preferences like [[Perfect Complements Utility Function|perfect complements]], the MRS is undefined at the kink. The optimality condition becomes:
$$x_1^* = x_2^*$$

#### Corner Solutions
When the tangency condition cannot be satisfied within the feasible region, use the appropriate [[Optimality Conditions for Corner Solutions|corner solution conditions]].

### Economic Interpretation
This mathematical framework captures the economic principle that individuals choose the bundle that maximizes their well-being subject to their budget constraint - the essence of [[Behavioral Postulate and Rational Choice|rational choice]].

### Applications by Preference Type
- [[Cobb-Douglas Demand Functions|Cobb-Douglas]]: Always interior, tractable algebra
- [[Perfect Substitutes Demand Functions|Perfect substitutes]]: Often corner, depends on price ratios
- [[Quasi-Linear Utility Function|Quasi-linear]]: Mixed interior/corner depending on parameters

---
#### Sources
[[MicroChapter5.pdf]]
#### Class
[[Microeconomics]]