## Feasibility and Optimality Conditions

The solution to [[Constrained Optimal Choice]] requires satisfying two fundamental conditions simultaneously.

### Feasibility Condition

**Definition**: The chosen bundle must be affordable given the consumer's budget constraint.

**Mathematical Form**:
$$p_1x_1^* + p_2x_2^* = m$$

**Economic Interpretation**: The consumer spends their entire income on the optimal bundle. This assumes no saving and complete expenditure of the budget.

**Graphical Representation**: The optimal bundle lies exactly on the budget line, not inside the budget set.

### Optimality Condition

The optimality condition varies by preference type and solution type ([[Interior and Corner Solutions]]).

#### For Interior Solutions with Differentiable Utility

**Tangency Condition**:
$$MRS(x^*) = \frac{p_1}{p_2}$$

**Alternative Forms**:
- Marginal utility ratio: $\frac{MU_{x_1}}{MU_{x_2}} = \frac{p_1}{p_2}$
- Equal marginal utility per dollar: $\frac{MU_{x_1}}{p_1} = \frac{MU_{x_2}}{p_2}$

**Economic Interpretation**: At the optimum, the rate at which the consumer is willing to substitute goods ([[Marginal Rate of Substitution|MRS]]) equals the rate at which the market allows substitution (relative prices).

#### For Interior Solutions with Non-Differentiable Utility

**Example**: [[Perfect Complements]]
- Standard tangency condition doesn't apply due to kinked indifference curves
- **Condition**: $x_1^* = x_2^*$ (equal consumption of both goods)
- Combined with feasibility: solve $p_1x + p_2x = m$ where $x = x_1^* = x_2^*$

#### For Corner Solutions

**Condition**: The [[Marginal Rate of Substitution|MRS]] is not equal to the price ratio.

**Case 1**: Consumer only good 1 ($x_1^* > 0, x_2^* = 0$)
$$MRS(x^*) > \frac{p_1}{p_2}$$

**Case 2**: Consumer only good 2 ($x_1^* = 0, x_2^* > 0$)
$$MRS(x^*) < \frac{p_1}{p_2}$$

**Economic Interpretation**: The consumer's willingness to trade differs sufficiently from market rates that they choose to consume only one good.

### Solution Method

1. **Identify preference type** and corresponding optimality condition
2. **Set up system of equations**:
   - Optimality condition (varies by type)
   - Feasibility condition: $p_1x_1 + p_2x_2 = m$
3. **Solve simultaneously** for $x_1^*$ and $x_2^*$ as functions of $(p_1, p_2, m)$
4. **Verify solution** satisfies both conditions

### Economic Intuition

These conditions ensure that:
- **Feasibility**: The choice is realistic given budget constraints
- **Optimality**: No other affordable bundle provides higher utility
- **Equilibrium**: Consumer has no incentive to change their choice

Together, they characterize the rational choice predicted by [[Rational Choice Theory]].

---
#### Sources
[[MicroChapter5.pdf]]
#### Class
[[Microeconomics]]