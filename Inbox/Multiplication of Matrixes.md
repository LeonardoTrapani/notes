To find each element in the resulting matrix, you take the dot product of a row from the first matrix with a column from the second matrix.

For element (i,j) in the result matrix C: C[i,j] = (row i of A) · (column j of B)

This means you multiply corresponding elements and sum them up: C[i,j] = A[i,1] × B[1,j] + A[i,2] × B[2,j] + ... + A[i,n] × B[n,j]

## Simple Example

Let's multiply two 2×2 matrices:

```
A = [1  2]    B = [5  6]
    [3  4]        [7  8]
```

To find C = A × B:

- C[1,1] = (1×5) + (2×7) = 5 + 14 = 19
- C[1,2] = (1×6) + (2×8) = 6 + 16 = 22
- C[2,1] = (3×5) + (4×7) = 15 + 28 = 43
- C[2,2] = (3×6) + (4×8) = 18 + 32 = 50

So C = [19 22] [43 50]

## Key Properties

- Matrix multiplication is **not commutative**: A×B ≠ B×A (in general)
- It **is associative**: (A×B)×C = A×(B×C)
- It's **distributive**: A×(B+C) = A×B + A×C