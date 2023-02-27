**Table of Contents**

- [Inverse of a matrix](#inverse-of-a-matrix)
  - [Finding the inverse matrix](#finding-the-inverse-matrix)


# Inverse of a matrix

Because the division operation can't be done with matrices, the concept of the inverse of a matrix was defined as noted below:

$$
A \cdot A^{-1} = I
$$

**_Note:_** Only square matrices with $\det{A} \ne 0$ have invert counterparts;

## Finding the inverse matrix

1. Check if matrix is invertible;
2. Create the [Augmented matrix]("https://www.en.wikipedia.org/wiki/Augmented_matrix") $(A|I)$;

  $$
  (A|I) = \left[
  \begin{array}{ccc|ccc}
  1 & -1 & -1 & 1 & 0 & 0\\
  -1 & 2 & 3 & 0 & 1 & 0\\
  1 & 1 & 4 & 0 & 0 & 1\\
  \end{array}
  \right]
  $$

3. Perform row operations (row addition, row subtraction and multiplication by a scalar) to transform the left side of the augmented matrix into the identity matrix;

    1.  $(A|I)_{1\,:} + (A|I)_{2\,:} \rightarrow (A|I)_{2\,:}$
    
    $$
    (A|I) = \left[
    \begin{array}{ccc|ccc}
    1 & -1 & -1 & 1 & 0 & 0\\
    0 & 1 & 2 & 1 & 1 & 0\\
    1 & 1 & 4 & 0 & 0 & 1\\
    \end{array}
    \right]
    $$
    
   2. $(A|I)_{3\,:} - (A|I)_{1\,:} \rightarrow (A|I)_{3\,:}$
    
    $$
    (A|I) = \left[
    \begin{array}{ccc|ccc}
    1 & -1 & -1 & 1 & 0 & 0\\
    0 & 1 & 2 & 1 & 1 & 0\\
    0 & 2 & 5 & -1 & 0 & 1\\
    \end{array}
    \right]
    $$
   
   3. $(A|I)_{1\,:} - (A|I)_{2\,:} \rightarrow (A|I)_{1\,:}$
    
    $$
    (A|I) = \left[
    \begin{array}{ccc|ccc}
    1 & 0 & 1 & 2 & 1 & 0\\
    0 & 1 & 2 & 1 & 1 & 0\\
    0 & 2 & 5 & -1 & 0 & 1\\
    \end{array}
    \right]
    $$
    
   4. $(A|I)_{3\,:} - (A|I)_{1\,:} \rightarrow (A|I)_{3\,:}$
    
    $$
    (A|I) = \left[
    \begin{array}{ccc|ccc}
    1 & -1 & -1 & 1 & 0 & 0\\
    0 & 1 & 2 & 1 & 1 & 0\\
    0 & 0 & 1 & -3 & -2 & 1\\
    \end{array}
    \right]
    $$

   5. $(A|I)_{1\,:} + (A|I)_{3\,:} \rightarrow (A|I)_{1\,:}$
    
    $$
    (A|I) = \left[
    \begin{array}{ccc|ccc}
    1 & 0 & 0 & 5 & 3 & -1\\
    0 & 1 & 2 & 1 & 1 & 0\\
    0 & 0 & 1 & -3 & -2 & 1\\
    \end{array}
    \right]
    $$

   6. $(A|I)_{2\,:} - 2 \cdot (A|I)_{3\,:} \rightarrow (A|I)_{2\,:}$
    
    $$
    (A|I) = \left[
    \begin{array}{ccc|ccc}
    1 & 0 & 0 & 5 & 3 & -1\\
    0 & 1 & 0 & 7 & 5 & -2\\
    0 & 0 & 1 & -3 & -2 & 1\\
    \end{array}
    \right]
    $$

4. The left side of the augmented matrix is equivalent to $A^{-1}$

$$
A^{-1} = \begin{bmatrix}
    5 & 3 & -1\\
    7 & 5 & -2\\
    -3 & -2 & 1\\
\end{bmatrix}
