**Table of contents**

- [Types of linear systems](#types-of-linear-systems)
- [Representing linear systems with matrices](#representing-linear-systems-with-matrices)
- [Solving linear systems](#solving-linear-systems)
  - [Inversion method](#inversion-method)
  - [Gaussian elimination](#gaussian-elimination)

# Types of linear systems

- Undetermined: Fewer equations than unknowns (Either has none or an infinite number of solutions);
- Determined: Same number of equations as unknowns (Has only one solution)
- Overdetermined: More equations that unknowns (Has no solution, but one can find the best approximate solution using linear regression) 

# Representing linear systems with matrices

A system of linear equations can be summarized as the following:

$$
A \cdot X = b
$$

1. The matrix of the coefficients;

$$
A = \begin{bmatrix}
    a_1 & b_1 & c_1 & \text{...} & z_1 \\
    a_2 & b_2 & c_2 & \text{...} & z_2 \\
    a_3 & b_3 & c_3 & \text{...} & z_3 \\  
    \text{...} & \text{...} & \text{...} & \text{...} & \text{...}\\  
    a_n & b_n & c_n & \text{...} & z_n \\  
\end{bmatrix}
$$

2. The matrix of the unknowns;

$$
X = \begin{bmatrix}
    x \\
    y \\
    z \\
    \text{...}\\
    w
\end{bmatrix}
$$

3. The matrix of the constants;

$$
b = \begin{bmatrix}
    K \\
    L \\
    M \\
    \text{...}\\
    J\\
\end{bmatrix}
$$

# Solving linear systems

## Inversion method

$$
X = A^{-1} \cdot b
$$

## Gaussian elimination

To solve the linear system using gaussian elimination, one must follow the steps listed below:

1. Create augmented matrix $(A|b)$;

$$
(A|b) = \left[
    \begin{array}{ccc|c}
    3 & -2 & 1 & 2\\
    4 & 3 & -2 & 4\\
    5 & -3 & 3 & 8\\
    \end{array}
    \right]
$$

2. Find the equivalent linear system with the row echelon form;

$$
\left[
    \begin{array}{ccc|c}
    3 & -2 & 1 & 2\\
    4 & 3 & -2 & 4\\
    5 & -3 & 3 & 8\\
    \end{array}
    \right]
\sim
\left[
    \begin{array}{ccc|c}
    3 & -2 & 1 & 2\\
    0 & 17 & -10 & 4\\
    0 & 0 & 78 & 234\\
    \end{array}
    \right]
$$

3. Solve using the resulting system using the substitution method;

$$
\begin{matrix}
3x & -2y & 1z & = & 2\\
    & 17y & -10z & = & 4\\
    &  & 78z & = & 234\\
\end{matrix}
\implies
\{(x,y,z)\} = \{(1, 2, 3)\}
$$