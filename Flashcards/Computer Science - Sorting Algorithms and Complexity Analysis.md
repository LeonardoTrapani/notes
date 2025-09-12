Source: [[Sorting Algorithms Index]]

# Computer Science - Sorting Algorithms and Complexity Analysis

#flashcards/computer-science/sorting-algorithms

## Sorting Problem Definition

What is the formal definition of the sorting problem?
?
**Input:** sequence ⟨a₁, a₂, ..., aₙ⟩ of numbers
**Output:** permutation ⟨a'₁, a'₂, ..., a'ₙ⟩ such that a'₁ ≤ a'₂ ≤ ... ≤ a'ₙ

The output must be a **permutation** (rearrangement) of the input elements arranged in non-decreasing order.
Source: [[Sorting Problem Definition]]

## Running Time Analysis Principles

What are the three key principles of running time analysis?
?
1. **Input Dependency**: Running time depends on input characteristics (sorted vs unsorted, size)
2. **Size Parametrization**: Parametrize running time by input size n since short sequences are easier to sort
3. **Upper Bound Focus**: Generally seek upper bounds because everybody likes a guarantee

Source: [[Running Time Analysis Principles]]

What is the "Big Idea" behind machine-independent algorithm analysis?
?
**Machine-Independent Analysis:**
- Ignore machine-dependent constants (use conventional unit cost for elementary operations)
- Look at growth of T(n) as n → ∞
- This approach is called **"Asymptotic Analysis"**

This enables meaningful algorithm comparison across different computing platforms.
Source: [[Running Time Analysis Principles]]

## Types of Algorithm Analysis

Define worst-case analysis and explain why it's preferred.
?
**Worst-Case Analysis:** T(n) = maximum time of algorithm on any input of size n

**Why preferred:**
- Most commonly used in practice
- Provides guaranteed performance bounds  
- Essential for critical applications
- No cheating with lucky inputs

Source: [[Types of Algorithm Analysis]]

Define average-case analysis and its requirements.
?
**Average-Case Analysis:** T(n) = expected time of algorithm over all inputs of size n

**Requirements:**
- Needs assumption of statistical distribution of inputs
- More complex to analyze
- Useful when input distribution is known

Source: [[Types of Algorithm Analysis]]

Why is best-case analysis considered "bogus"?
?
**Problems with best-case analysis:**
- Can cheat with a slow algorithm that works fast on some specific input
- Doesn't provide meaningful performance guarantees
- Generally not useful for practical algorithm evaluation
- Can be misleading about real performance

Source: [[Types of Algorithm Analysis]]

## Asymptotic Notation (Θ-notation)

What is the mathematical definition of Θ-notation?
?
f(n) = Θ(g(n)): there exist positive constants c₁, c₂, and n₀ such that

**0 ≤ c₁g(n) ≤ f(n) ≤ c₂g(n)** for all n ≥ n₀

This means f(n) is bounded both above and below by g(n) up to constant factors.
Source: [[Asymptotic Notation]]

What is the practical approach for applying Θ-notation?
?
**For practitioners:**
1. **Drop low-order terms**
2. **Ignore leading constants**

**Example:** 3n³ + 90n² - 5n + 6046 = Θ(n³)

The dominant term (highest degree) determines the asymptotic complexity.
Source: [[Asymptotic Notation]]

Complete this key principle: "When n gets large enough, a Θ(n²) algorithm _____ a Θ(n³) algorithm."
?
"When n gets large enough, a Θ(n²) algorithm **always beats** a Θ(n³) algorithm."

This demonstrates the power of asymptotic analysis - the dominant growth factor eventually outweighs constant factors and lower-order terms.
Source: [[Asymptotic Notation]]

## Insertion Sort Algorithm

What is the core intuition behind insertion sort?
?
**Intuition:** Move smaller numbers to the left by inserting each element into its correct position within the already sorted portion.

Like sorting playing cards in your hand - take each new card and insert it in the right spot among the already sorted cards.
Source: [[Insertion Sort Algorithm]]

Write the pseudocode for insertion sort.
?
```
INSERTION-SORT (A, n) ⊳ A[1..n]
for j ← 2 to n
    do key ← A[j]
       i ← j - 1
       while i > 0 and A[i] > key
           do A[i+1] ← A[i]
              i ← i - 1
       A[i+1] = key
```

Note: `x ← y` means "assign value y to variable x"
Source: [[Insertion Sort Algorithm]]

List the 5 steps of the insertion sort algorithm.
?
1. **Start from position 2** (since single element is already sorted)
2. **Select current element** as `key`  
3. **Scan backwards** through the sorted portion
4. **Shift elements** greater than `key` to the right
5. **Insert key** in the correct position

Source: [[Insertion Sort Algorithm]]

What are the four key characteristics of insertion sort?
?
1. **In-place sorting:** Uses constant extra memory
2. **Stable:** Preserves relative order of equal elements
3. **Online:** Can sort elements as they arrive  
4. **Adaptive:** Efficient on already sorted or nearly sorted data

Source: [[Insertion Sort Algorithm]]

## Insertion Sort Complexity Analysis

What is the worst-case scenario for insertion sort and its complexity?
?
**Scenario:** Input reverse sorted

**Time Complexity:** T(n) = Σ(j=2 to n) Θ(j) = **Θ(n²)**

This follows from the arithmetic series formula (discovered by Gauss at 6 years old).
Source: [[Insertion Sort Complexity Analysis]]

What is insertion sort's average-case complexity and assumption?
?
**Assumption:** All permutations equally likely

**Time Complexity:** T(n) = Σ(j=2 to n) Θ(j/2) = **Θ(n²)**

The average case has the same asymptotic complexity as worst case, differing only by a constant factor.
Source: [[Insertion Sort Complexity Analysis]]

For what input sizes is insertion sort considered fast vs slow?
?
**Fast:** Moderately fast for **small n** (typically n < 30)
**Slow:** Not fast at all for **large n**

**Key insight:** Quadratic growth makes it impractical for large datasets, but simplicity makes it useful for small inputs.
Source: [[Insertion Sort Complexity Analysis]]

## Merge Sort Algorithm  

What algorithmic paradigm does merge sort follow?
?
**Merge Sort** follows the **divide-and-conquer paradigm**.

It recursively breaks problems into smaller subproblems, solves them independently, and combines the solutions.
Source: [[Merge Sort Algorithm]]

Write the elegant recursive pseudocode for merge sort.
?
```
MERGE-SORT (A[1..n])
{ if n > 1
    MERGE-SORT (A[1..⌈n/2⌉])
    MERGE-SORT (A[⌈n/2⌉+1..n])  
    MERGE(A[1..n])
}
```

The base case (n = 1) is implicitly handled when the condition n > 1 is false.
Source: [[Merge Sort Algorithm]]

Explain the three steps of merge sort's divide-and-conquer strategy.
?
1. **Divide:** Split the n-element array A into 2 subarrays of n/2 elements each
2. **Conquer:** Recursively sort the two subarrays
3. **Combine:** Merge 2 sorted subarrays into 1 sorted array

The critical **MERGE** operation combines two sorted arrays in Θ(n) time.
Source: [[Merge Sort Algorithm]]

What are the four main advantages of merge sort?
?
1. **Guaranteed O(n log n) performance** in all cases
2. **Stable sorting** preserves relative order of equal elements
3. **Predictable performance** regardless of input distribution  
4. **Recursive structure** makes it elegant and easy to analyze

Source: [[Merge Sort Algorithm]]

## Merge Sort Complexity Analysis

Write the recurrence relation for merge sort's time complexity.
?
T(n) = {
  Θ(1)           if n = 1
  2T(n/2) + Θ(n) if n > 1
}

**Components:**
- **Base case:** Θ(1) for single element
- **Recursive calls:** 2T(n/2) for sorting two halves  
- **Merge operation:** Θ(n) for combining results

Source: [[Merge Sort Complexity Analysis]]

Using the recursion tree method, solve T(n) = 2T(n/2) + cn.
?
**Tree Structure:**
- **Height:** h = lg n
- **Work per level:** cn (constant across all levels)
- **Number of levels:** lg n + 1
- **Leaves:** n nodes, each requiring Θ(1) work

**Solution:** Total = cn × (lg n + 1) + Θ(n) = **Θ(n lg n)**
Source: [[Merge Sort Complexity Analysis]]

What is merge sort's time complexity in all cases, and what's the practical crossover point?
?
**Time Complexity:** **Θ(n lg n)** in worst, average, and best cases

**Practical Crossover:** Merge sort beats insertion sort for **n > 30** or so

**Key insight:** Θ(n lg n) grows more slowly than Θ(n²), making merge sort asymptotically superior.
Source: [[Merge Sort Complexity Analysis]]

## Divide and Conquer Paradigm

What is the three-step process of divide-and-conquer algorithms?
?
1. **Divide:** Break the problem into several subproblems that are similar to the original but smaller in size
2. **Conquer:** Solve the subproblems recursively. If small enough, solve directly (base case)
3. **Combine:** Merge the solutions of subproblems into a solution for the original problem

Source: [[Divide and Conquer Algorithms]]

What are the four key characteristics of divide-and-conquer algorithms?
?
1. **Recursive structure** naturally leads to elegant solutions
2. **Parallel potential** - subproblems can often be solved independently
3. **Optimal complexity** for many problems (like sorting)
4. **Mathematical analysis** through recurrence relations

Source: [[Divide and Conquer Algorithms]]

How does merge sort exemplify the divide-and-conquer paradigm?
?
**Merge Sort Example:**
1. **Divide:** Split n-element array into 2 subarrays of n/2 elements each
2. **Conquer:** Recursively sort the two subarrays  
3. **Combine:** Merge 2 sorted subarrays into 1 sorted array

This perfectly illustrates all three steps of the paradigm.
Source: [[Divide and Conquer Algorithms]]

## Recurrence Relations

What is a recurrence relation in the context of algorithm analysis?
?
A **recurrence relation** expresses a function in terms of its values on smaller inputs, providing a mathematical framework for analyzing recursive algorithms.

It captures both the recursive structure and the work done at each level.
Source: [[Recurrence Relations]]

What is the general form of recurrence relations for divide-and-conquer algorithms?
?
T(n) = {
  base case                                                           if n ≤ n₀
  combination of T(smaller inputs) + work at current level           otherwise  
}

This structure captures the recursive decomposition and combination costs.
Source: [[Recurrence Relations]]

Using the recursion tree method, what are the four key steps to solve T(n) = 2T(n/2) + cn?
?
1. **Tree height:** h = lg n
2. **Work per level:** cn (constant across all levels)  
3. **Total levels:** lg n + 1
4. **Leaf contribution:** Θ(n)

**Solution:** T(n) = Θ(n lg n)

The recursion tree visualizes work distribution across recursion levels.
Source: [[Recurrence Relations]]

## Algorithm Comparison

Complete this comparison table for insertion sort vs merge sort:

| Algorithm | Best Case | Average Case | Worst Case | Space |
|-----------|-----------|--------------|------------|-------|
| Insertion Sort | ? | ? | ? | ? |
| Merge Sort | ? | ? | ? | ? |
?
| Algorithm | Best Case | Average Case | Worst Case | Space |
|-----------|-----------|--------------|------------|-------|
| Insertion Sort | Θ(n) | Θ(n²) | Θ(n²) | Θ(1) |
| Merge Sort | Θ(n lg n) | Θ(n lg n) | Θ(n lg n) | Θ(n) |

Source: [[Sorting Algorithms Comparison]]

What are the three main advantages of merge sort over insertion sort?
?
1. **Guaranteed Θ(n lg n) performance** regardless of input
2. **Predictable behavior** for critical applications
3. **Efficient for large datasets** due to better asymptotic complexity

Source: [[Sorting Algorithms Comparison]]

What are the four main advantages of insertion sort over merge sort?
?
1. **Simple implementation** - easier to code and understand
2. **Low overhead** for small arrays  
3. **In-place sorting** - uses constant extra space Θ(1)
4. **Better for n < 30** approximately due to lower constants

Source: [[Sorting Algorithms Comparison]]

At approximately what input size does merge sort begin to outperform insertion sort?
?
**Crossover Point:** Merge sort beats insertion sort for **n > 30** or so.

**Practical optimization:** Many implementations use insertion sort for small subarrays within merge sort to take advantage of both algorithms' strengths.
Source: [[Sorting Algorithms Comparison]]

What are the four key guidelines for algorithm selection between insertion sort and merge sort?
?
1. **Small datasets:** Insertion sort may be preferable
2. **Large datasets:** Merge sort provides better scalability
3. **Guaranteed performance:** Merge sort offers consistent behavior  
4. **Memory constraints:** Insertion sort uses less space

Algorithm choice depends on both theoretical complexity and practical implementation considerations.
Source: [[Sorting Algorithms Comparison]]

## Synthesis and Key Insights

Why do Θ(n lg n) algorithms eventually beat Θ(n²) algorithms for large inputs?
?
**Asymptotic Growth Comparison:**
- Θ(n lg n) grows **more slowly** than Θ(n²) as n increases
- For large n, the difference becomes **dramatically significant**
- **Example:** For n = 1,000,000: n lg n ≈ 20M vs n² ≈ 1T operations

This demonstrates the power of asymptotic analysis in predicting algorithm scalability.
Source: [[Asymptotic Notation]], [[Sorting Algorithms Comparison]]

What fundamental insight does the comparison between insertion sort and merge sort teach about algorithm design?
?
**Key Insights:**
1. **Simple algorithms** (insertion sort) can be better for small inputs
2. **Sophisticated algorithms** (merge sort) scale better for large inputs  
3. **Asymptotic analysis** predicts long-term performance
4. **Real-world optimization** often combines multiple approaches

**Broader principle:** Algorithm choice requires balancing theoretical complexity with practical implementation considerations.
Source: [[Sorting Algorithms Comparison]]

How does the study of sorting algorithms demonstrate the importance of different analysis techniques?
?
**Analysis Techniques Demonstrated:**
1. **Worst-case analysis** - provides performance guarantees
2. **Asymptotic notation** - enables algorithm comparison
3. **Recurrence relations** - analyzes recursive algorithms
4. **Recursion trees** - visualizes complexity analysis

**Integration:** These techniques work together to provide comprehensive understanding of algorithm behavior and enable informed design decisions.
Source: [[Types of Algorithm Analysis]], [[Asymptotic Notation]], [[Recurrence Relations]]