Source: [[To Review/Microeconomics/]]

#flashcards/microeconomics/core

## Utility Theory Fundamentals

What is a utility function and what does it represent?
?
A utility function $u(x)$ assigns numerical values that reflect the relative rankings of various bundles of goods. It represents a preference relation where:
- $a \succeq b \Leftrightarrow u(a) \geq u(b)$ 
- $a \succ b \Leftrightarrow u(a) > u(b)$
- $a \sim b \Leftrightarrow u(a) = u(b)$

The key insight is that utility functions are **ordinal** - only the ranking matters, not absolute values.

---

What is marginal utility and how is it calculated mathematically?
?
**Marginal utility** of good $x_i$ is the change in utility from consuming one more unit of good $x_i$.

Mathematical representation:
- Discrete: $MU_{x_i} = \frac{\Delta U}{\Delta x_i}$
- Continuous: $MU_{x_i} = \frac{\partial U}{\partial x_i}$

Marginal utility is the **slope** of the utility function with respect to good $x_i$.

---

How does marginal utility relate to the marginal rate of substitution?
?
The marginal rate of substitution can be expressed in terms of marginal utilities:

$$MRS = -\frac{MU_{x_1}}{MU_{x_2}}$$

**Derivation**: On the same indifference curve, $MU_{x_1} dx_1 + MU_{x_2} dx_2 = 0$

Rearranging: $\frac{dx_2}{dx_1} = -\frac{MU_{x_1}}{MU_{x_2}} = MRS$

---

## Consumer Preferences and Choice

What are the five preference axioms and what does each represent?
?
1. **Completeness**: "Always have an answer" - can compare any two bundles
2. **Reflexivity**: Any bundle is at least as good as itself 
3. **Transitivity**: "Avoid contradictory answers" - if $b \succeq a$ and $c \succeq b$, then $c \succeq a$
4. **Monotonicity**: "More is better" - bundles with more of at least one good are preferred
5. **Convexity**: "People prefer variety to extremes" - averages of equally preferred bundles are at least as good

---

What is the Marginal Rate of Substitution (MRS) and what does it measure?
?
The **MRS** is the ratio at which a consumer is **willing to trade** one good for another while remaining equally satisfied.

- Mathematical definition: $MRS = \frac{dx_2}{dx_1}$ (slope of indifference curve)
- Economic interpretation: Maximum quantity of good 2 the consumer will give up to get one additional unit of good 1
- Key property: For well-behaved preferences, MRS is diminishing (absolute value decreases as $x_1$ increases)

---

## Budget Constraints and Optimization

What is the budget constraint and how is it mathematically expressed?
?
The **budget constraint** identifies bundles a consumer can **just afford** (spending all income):

$$p_1 x_1 + p_2 x_2 = m$$

In slope-intercept form: $x_2 = \frac{m}{p_2} - \frac{p_1}{p_2}x_1$

Key components:
- Vertical intercept: $\frac{m}{p_2}$
- Horizontal intercept: $\frac{m}{p_1}$  
- Slope: $-\frac{p_1}{p_2}$ (opportunity cost)

---

What are the conditions for constrained optimal choice?
?
For an optimal bundle $x^*$, two conditions must hold:

1. **Feasibility condition**: $p_1x_1^* + p_2x_2^* = m$
2. **Optimality condition**: $MRS(x^*) = \frac{p_1}{p_2}$

**Economic intuition**: "How much I MUST trade off" (price ratio) equals "how much I WANT to trade off" (MRS).

Equivalently: $\frac{MU_{x_1}}{MU_{x_2}} = \frac{p_1}{p_2}$ or $\frac{MU_{x_1}}{p_1} = \frac{MU_{x_2}}{p_2}$

---

What distinguishes interior solutions from corner solutions in consumer optimization?
?
**Interior Solution**: Consumer chooses both goods ($x_1^* > 0$ and $x_2^* > 0$)
- Condition: $MRS(x^*) = \frac{p_1}{p_2}$ (tangency condition)

**Corner Solution**: Consumer chooses only one good
- $x_1^* > 0, x_2^* = 0$: when $MRS(x^*) > \frac{p_1}{p_2}$
- $x_1^* = 0, x_2^* > 0$: when $MRS(x^*) < \frac{p_1}{p_2}$

---

## Specific Utility Functions

What are the key properties of Cobb-Douglas utility functions?
?
**General form**: $u(x_1, x_2) = x_1^a x_2^b$ with $a > 0, b > 0$

**Properties**:
- Always well-behaved (satisfy all 5 preference axioms)
- Indifference curves are hyperbolic
- Never touch axes (both goods always consumed)
- Exhibit diminishing MRS

**MRS formula**: $MRS = -\frac{a x_2}{b x_1}$

**Special case**: $u(x_1, x_2) = x_1 x_2 \Rightarrow MRS = -\frac{x_2}{x_1}$

---

Perfect Substitutes vs Perfect Complements: What are their key characteristics?
?
**Perfect Substitutes**:
- Utility: $U(x_1, x_2) = ax_1 + bx_2$
- Indifference curves: Straight lines (constant MRS)
- Behavior: Corner solutions (choose cheaper good)
- Axiom violated: Strict convexity

**Perfect Complements**: 
- Utility: $U(x_1, x_2) = \min\{x_1/a, x_2/b\}$
- Indifference curves: L-shaped with kinks
- Behavior: Fixed proportion consumption
- MRS: Zero on horizontal segments, infinite on vertical segments

---

## Demand Analysis

What are Marshallian demand functions and how are they derived?
?
**Marshallian demand functions** are optimal consumption choices from solving:
$$\max_{x_1, x_2} U(x_1, x_2) \text{ subject to } p_1x_1 + p_2x_2 = m$$

Results in demand functions: $x_1^*(p_1, p_2, m)$ and $x_2^*(p_1, p_2, m)$

**Properties**:
- Depend on all prices and income
- Represent utility-maximizing choices
- Different utility functions generate different demand forms
- Monotonic transformations yield identical demands

---

How do you distinguish between normal goods, inferior goods, ordinary goods, and Giffen goods?
?
**By income response**:
- **Normal goods**: $\frac{\partial x_1^*}{\partial m} > 0$ (demand increases with income)
- **Inferior goods**: $\frac{\partial x_1^*}{\partial m} < 0$ (demand decreases with income)

**By own-price response**:
- **Ordinary goods**: $\frac{\partial x_1^*}{\partial p_1} < 0$ (demand decreases with own price)
- **Giffen goods**: $\frac{\partial x_1^*}{\partial p_1} > 0$ for some price ranges (demand increases with own price)

**Note**: Giffen goods are a subset of inferior goods where income effects dominate substitution effects.

---

## Advanced Utility Functions and Concepts

What is a quasi-linear utility function and what are its key properties?
?
**Quasi-linear utility function**: $u(x_1, x_2) = f(x_1) + x_2$ (linear in $x_2$ only)

**Key properties**:
- Marginal utilities: $MU_{x_1} = f'(x_1)$ and $MU_{x_2} = 1$
- MRS: $MRS = -f'(x_1)$ (depends only on $x_1$, not $x_2$)
- Indifference curves: Vertically shifted copies of each other
- Economic interpretation: Often used when $x_2$ represents money (constant marginal utility of money)

**Example**: $u(x_1, x_2) = 2x_1^{1/2} + x_2$

---

What is an Engel curve and how does it relate to goods classification?
?
An **Engel curve** plots quantity demanded against income, holding prices constant: $x_1^* = f(m | p_1, p_2)$

**Characteristics by good type**:
- **Normal goods**: Positively sloped ($\frac{\partial x_1^*}{\partial m} > 0$)
- **Inferior goods**: Negatively sloped ($\frac{\partial x_1^*}{\partial m} < 0$)

**Construction**: Derived from income offer curve by plotting quantity-income pairs

**Economic significance**: Shows how consumption patterns change with income levels - steep slope indicates luxury goods, gentle slope indicates necessities.

---

How do you distinguish between gross substitutes and gross complements?
?
Classification based on cross-price effects:

**Gross Substitutes**: $\frac{\partial x_1^*}{\partial p_2} > 0$
- When $p_2$ increases, demand for good 1 increases
- Goods can replace each other (coffee/tea, butter/margarine)
- Demand curve for good 1 shifts outward when $p_2$ rises

**Gross Complements**: $\frac{\partial x_1^*}{\partial p_2} < 0$ 
- When $p_2$ increases, demand for good 1 decreases
- Goods are consumed together (cars/gasoline, printers/ink)
- Demand curve for good 1 shifts inward when $p_2$ rises

**Unrelated goods**: $\frac{\partial x_1^*}{\partial p_2} = 0$

---

## Utility Theory Extensions

What are monotonic transformations and why do they preserve preferences?
?
**Monotonic transformations** apply strictly increasing functions to utility values.

**Definition**: If $u$ is a utility function and $f$ is strictly increasing, then $V = f(u)$ represents the same preferences.

**Key properties**:
- Preserve preference ordering between bundles
- Preserve indifference relationships  
- **Do not change MRS** - MRS is invariant under monotonic transformations
- Examples: $V = u^2$, $V = 2u + 10$, $V = \ln(u)$ (when $u > 0$)

**Economic significance**: Since utility is ordinal, any strictly increasing transformation yields identical choice behavior.

---

How do ordinal and cardinal utility differ conceptually?
?
**Ordinal utility**: Only **rankings** matter, not absolute values
- Tells us IF one bundle is preferred to another
- Scale is arbitrary - only ordering preserved
- Standard assumption in microeconomics
- Example: $u(a) = 6, u(b) = 2$ means $a \succ b$, but NOT "3 times better"

**Cardinal utility**: **Magnitudes** of utility differences matter
- Tells us HOW MUCH better one alternative is
- Requires meaningful numerical scale
- Not typically assumed in consumer theory
- Example: Bundle A provides "twice as much satisfaction" as Bundle B

**Historical note**: Ordinal approach established by Vilfredo Pareto (1848-1923).

---

## Advanced Preference Types

How do you distinguish between goods, bads, and neutrals in utility theory?
?
Classification based on **marginal utility** signs:

**Good**: $MU > 0$
- Increases utility with additional consumption
- "More is better" - consumer prefers more to less
- Examples: food, entertainment, housing

**Bad**: $MU < 0$ 
- Decreases utility with additional consumption
- Consumer prefers less to more
- Examples: pollution, noise, disease

**Neutral**: $MU = 0$
- No change in utility from additional consumption
- Consumer indifferent to having more or less
- Examples: worthless objects, items beyond satiation

**Graphical implication**: Goods create downward-sloping indifference curves; bads create upward-sloping curves.

---

What are concave preferences and how do they differ from standard convex preferences?
?
**Concave preferences** have indifference curves that are "bowed outward" toward the origin.

**Key characteristics**:
- **Increasing MRS**: Marginal rate of substitution rises along the curve
- **Violates diminishing MRS**: Contradicts standard convexity assumption
- **Always corner solutions**: No interior optima exist
- **Specialization preferred**: Consumer chooses only one good

**Economic interpretation**: Models "addiction-like" behavior where more consumption makes a good relatively more desirable.

**Examples**: Technology adoption (network effects), habit formation, social conformity

**Contrast with convex preferences**: Standard theory assumes convex indifference curves (diminishing MRS, interior solutions preferred).

---

## Consumer Choice Analysis

What are the complete feasibility and optimality conditions for consumer choice?
?
Consumer optimization requires satisfying **both conditions simultaneously**:

**1. Feasibility Condition**: 
$$p_1x_1^* + p_2x_2^* = m$$
Consumer spends entire income on optimal bundle.

**2. Optimality Condition** (varies by case):
- **Interior solutions**: $MRS(x^*) = \frac{p_1}{p_2}$
- **Corner solution** (only good 1): $MRS(x^*) > \frac{p_1}{p_2}$  
- **Corner solution** (only good 2): $MRS(x^*) < \frac{p_1}{p_2}$
- **Perfect complements**: $x_1^* = x_2^*$ (equal consumption)

**Economic intuition**: Consumer's willingness to trade (MRS) must equal or be incompatible with market trade-off (price ratio).

---

## Demand Analysis Framework

What is comparative statics analysis in consumer theory?
?
**Comparative statics analysis** studies how optimal demand changes when parameters change.

**Three main types**:

1. **Own-price effects**: How does $x_1^*$ change as $p_1$ changes?
   - Generates price offer curves and demand functions
   
2. **Cross-price effects**: How does $x_1^*$ change as $p_2$ changes?
   - Determines if goods are substitutes or complements
   
3. **Income effects**: How does $x_1^*$ change as $m$ changes?
   - Generates income offer curves and Engel curves
   - Classifies goods as normal or inferior

**Significance**: Forms theoretical foundation for understanding market behavior and deriving demand relationships used in economic analysis.

---

What is the price offer curve and how is it constructed?
?
The **price offer curve** traces all optimal consumption bundles as one good's price varies.

**Construction**:
1. Fix $p_2$ and $m$ constant
2. Systematically vary $p_1$: $p_1' < p_1'' < p_1'''$
3. Find optimal bundle at each price using feasibility/optimality conditions
4. Connect all optimal points

**Key relationships**:
- **Direct foundation** for demand curves
- **Upper panel**: Shows bundles in $(x_1, x_2)$ space  
- **Lower panel**: Shows corresponding demand in $(p_1, x_1)$ space
- **Vertical lines** connect corresponding points between panels

**Shape varies by preference type**: Smooth curves (Cobb-Douglas), L-shaped segments (perfect complements), discontinuous jumps (perfect substitutes).

---

What is the price-consumption curve and how does it relate to consumer behavior?
?
The **price-consumption curve** is another name for the price offer curve - it traces optimal bundles as price varies.

**Economic interpretation**:
- Shows how consumers **substitute between goods** as relative prices change
- **Steep curves**: Limited substitutability
- **Flat curves**: High substitutability  
- **Kinked curves**: Threshold effects in substitution

**Income effects included**: Price changes affect real purchasing power, influencing consumption of both goods
- Normal goods: consumption decreases as effective income falls
- Inferior goods: consumption might increase as effective income falls

**Applications**: Predicting consumption changes from price policies, analyzing tax/subsidy effects, measuring consumer surplus changes.

---

## Demand Functions and Curves

How do direct and inverse demand functions differ?
?
**Direct demand function**: Quantity as function of price
$$x_1^* = f(p_1 | p_2, m)$$
- **Answers**: "Given price, what quantity is demanded?"
- **Standard form** for most economic analysis
- **Ordinary goods**: Downward-sloping
- **Giffen goods**: Can have upward-sloping segments

**Inverse demand function**: Price as function of quantity  
$$p_1 = g(x_1^* | p_2, m)$$
- **Answers**: "At what price would given quantity be demanded?"
- **Mathematical inverse** of direct demand
- **Actually plotted** when we draw demand curves (price on vertical axis)
- **Represents marginal willingness to pay** for each unit

**Key insight**: Standard demand curve graphs show inverse demand function despite being called "demand curve."

---

What is the income offer curve and how does it relate to Engel curves?
?
The **income offer curve** traces all optimal bundles as income varies, holding prices constant.

**Construction**:
1. Fix both prices $p_1$ and $p_2$ constant
2. Vary income levels: $m' < m'' < m'''$
3. Find optimal consumption bundle at each income level
4. Connect optimal points

**Shape characteristics**:
- **Both goods normal**: Slopes upward and outward
- **One good inferior**: Can bend backward as inferior good consumption decreases

**Direct relationship to Engel curves**:
- **$x_1$-coordinates** of income offer curve → Engel curve for good 1
- **$x_2$-coordinates** of income offer curve → Engel curve for good 2

**Example (Cobb-Douglas)**: Income offer curve is linear with slope $\frac{bp_1}{ap_2}$ (constant expenditure ratios).

---

## Good Classifications

How do ordinary goods differ from Giffen goods in terms of price responses?
?
**Ordinary goods**: Standard price-quantity relationship
- **Demand curve**: Always downward-sloping  
- **Price response**: $\frac{\partial x_1^*}{\partial p_1} < 0$ for all prices
- **Economic intuition**: Higher prices reduce quantity demanded
- **Prevalence**: Most goods in practice

**Giffen goods**: Paradoxical price-quantity relationship
- **Demand curve**: Has upward-sloping segments
- **Price response**: $\frac{\partial x_1^*}{\partial p_1} > 0$ for some price ranges
- **Economic intuition**: Strong income effects can overwhelm substitution effects
- **Requirements**: Must be inferior goods with large budget share and limited substitutes
- **Prevalence**: Extremely rare theoretical curiosity

**Price offer curves**: Ordinary goods show consistently leftward movement as price rises; Giffen goods can show backward-bending behavior.

---

## Integration and Applications

How do all these demand concepts integrate in consumer theory?
?
**Hierarchical relationship**:

1. **Preferences** → **Utility functions** (with monotonic transformation invariance)
2. **Utility maximization** → **Feasibility and optimality conditions**
3. **Optimal choice** → **Marshallian demand functions**
4. **Comparative statics** → **Offer curves** (price and income)
5. **Offer curves** → **Demand curves** and **Engel curves**

**Classification system**:
- **By income response**: Normal vs Inferior goods
- **By own-price response**: Ordinary vs Giffen goods  
- **By cross-price response**: Gross substitutes vs complements

**Analytical tools**:
- **Price-consumption curves**: Trace substitution patterns
- **Income offer curves**: Trace wealth effects
- **Direct/inverse demand**: Alternative representations
- **Engel curves**: Income-quantity relationships

**Foundation for market analysis**: Individual demand aggregates to market demand, enabling equilibrium and welfare analysis.