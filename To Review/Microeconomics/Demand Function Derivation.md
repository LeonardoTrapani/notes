## Overview

Demand function derivation is the process of obtaining demand curves from underlying consumer preferences and constraints through utility maximization.

## Theoretical Foundation

### Starting Point
1. **Consumer preferences** represented by [[Utility Functions]]
2. **Budget constraint**: $p_1x_1 + p_2x_2 = m$
3. **Optimization problem**: Maximize utility subject to budget constraint

### Optimization Process
The consumer solves:
$$\max_{x_1, x_2} u(x_1, x_2) \text{ subject to } p_1x_1 + p_2x_2 = m$$

Using [[Marginal Rate of Substitution|marginal conditions]]:
$$\frac{MU_1}{MU_2} = \frac{p_1}{p_2}$$

## Types of Demand Functions

### Ordinary Demand Functions
Solution to the utility maximization problem:
- $x_1^*(p_1, p_2, m)$ 
- $x_2^*(p_1, p_2, m)$

These show **optimal quantities** as functions of all prices and income.

### Marshallian Demand
Another name for ordinary demand functions, named after Alfred Marshall.

## Deriving Specific Functional Forms

### Cobb-Douglas Example
For $u(x_1, x_2) = x_1^a x_2^b$:

**Step 1**: Set up Lagrangian
$$\mathcal{L} = x_1^a x_2^b + \lambda(m - p_1x_1 - p_2x_2)$$

**Step 2**: First-order conditions
- $\frac{\partial \mathcal{L}}{\partial x_1} = ax_1^{a-1}x_2^b - \lambda p_1 = 0$
- $\frac{\partial \mathcal{L}}{\partial x_2} = bx_1^a x_2^{b-1} - \lambda p_2 = 0$

**Step 3**: Solve system to get:
- $x_1^* = \frac{am}{(a+b)p_1}$
- $x_2^* = \frac{bm}{(a+b)p_2}$

## Comparative Statics from Derived Demands

Once demand functions are derived, [[Comparative Statics Analysis]] examines:

### Own-Price Effects
$\frac{\partial x_1^*}{\partial p_1}$ → Determines if good is [[Ordinary and Giffen Goods|ordinary or Giffen]]

### Cross-Price Effects  
$\frac{\partial x_1^*}{\partial p_2}$ → Determines if goods are [[Gross Substitutes and Complements|substitutes or complements]]

### Income Effects
$\frac{\partial x_1^*}{\partial m}$ → Determines if good is [[Normal and Inferior Goods|normal or inferior]]

## From Individual to Market Demand

### Aggregation Process
Market demand = Sum of individual demands:
$$X_1^D(p_1, p_2) = \sum_{i=1}^n x_{1i}^*(p_1, p_2, m_i)$$

Where $n$ is the number of consumers.

## Graphical Derivation

### Price Offer Curve Method
1. Vary $p_1$ while holding $p_2, m$ constant
2. Find optimal bundles → [[Price Offer Curve]]
3. Extract $x_1^*$ coordinates → [[Direct Demand Function]]

### Income Offer Curve Method  
1. Vary $m$ while holding $p_1, p_2$ constant
2. Find optimal bundles → [[Income Offer Curve]]
3. Extract $x_1^*$ coordinates → [[Engel Curve]]

## Inverse Demand Derivation

From direct demand $x_1^* = f(p_1)$, solve for $p_1$:
$$p_1 = f^{-1}(x_1^*) \rightarrow \text{[[Inverse Demand Function]]}$$

## Applications

### Market Analysis
- Predicting consumer responses to price changes
- Revenue optimization for firms
- Policy impact assessment

### Welfare Economics
- Consumer surplus calculations
- Deadweight loss analysis
- Market efficiency evaluation

## Related Concepts

- [[Utility Functions]]
- [[Budget Constraints]]  
- [[Comparative Statics Analysis]]
- [[Rational Choice Theory]]

---
#### Sources
[[MicroChapter6.pdf]]
#### Class
[[Microeconomics]]