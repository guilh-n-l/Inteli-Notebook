**Table of contents**

- [Vectors](#vectors)
  - [Parametric representation of lines](#parametric-representation-of-lines)
  - [Linear combination](#linear-combination)
    - [Span](#span)
  - [Linear independence](#linear-independence)
  - [Subspace of a vector set](#subspace-of-a-vector-set)
  - [Vector transformations](#vector-transformations)
  - [Linear transformations](#linear-transformations)
  - [Null space](#null-space)
  - [Eigenvalues and eigenvectors](#eigenvalues-and-eigenvectors)
    - [Determining the matrix of eigenvalues of a matrix](#determining-the-matrix-of-eigenvalues-of-a-matrix)
      - [Using determinants](#using-determinants)
      - [Using the matrix of eigenvectors](#using-the-matrix-of-eigenvectors)
    - [Determining the eigenvectors using the eigenspace](#determining-the-eigenvectors-using-the-eigenspace)
    - [Determining the transformation matrix using eigenvalues and eigenvectors](#determining-the-transformation-matrix-using-eigenvalues-and-eigenvectors)

# Vectors 

## Parametric representation of lines

A line $(\mathbf{L})$ in an $n$ dimensional space can be represented using a vector equation, such as the one below:

$$
\mathbf{L} = \{k \cdot \vec{v};\, k \in \mathbb{R}\}
$$

## Linear combination

Given a set of vectors $(\mathbf{V})$ and a set of scalars $(\mathbf{C})$, a linear combination can be represented as below:

$$
\mathbf{V} = \left\{\vec{v_1}, \vec{v_2}, \vec{v_3}, ... \right\}
$$
$$
\mathbf{C} = \left\{c_1, c_2, c_3, ... \right\}
$$
$$
\left(c_1 \cdot \vec{v_1} + c_2 \cdot \vec{v_2} + c_3 \cdot \vec{v_3} +...\right) \text{ Is a linear combination of $\mathbf{C}\And\mathbf{V}$}
$$

### Span

The span of a set of vectors $\left(\text{Span}\left(\vec{v_1}, \vec{v_2}, \vec{v_3}, ...\right)\right)$ is the set of all possible linear combinations between that set of vectors and the set of real numbers;

## Linear independence

A set of vectors is said to be linearly independent if at least one vector in that set can't be represented as a linear combination of other vectors in that set;

Only if there is no solution for $(c_1 \cdot \vec{v_1} + c_2 \cdot \vec{v_2} + c_3 \cdot \vec{v_3} +... = 0)$ other than when $\forall c_i = 0$ that the set of vectors is linearly independent;

## Subspace of a vector set

A subset $\mathbf{U}$ is said to be a subspace of a superset $\mathbf{V}$ when $\mathbf{U}$ follows all the conditions below:

1. $\vec{0} \in U$
2. $\mathbf{U}$ contains all the linear combinations of vectors in itself (Is closed in vector addition and scalar multiplication)

**_Note:_** $\text{Span}(\mathbf{V})$ are always valid subspaces;

## Vector transformations

Vector transformations are the association between vectors from a $\mathbb{D}$ to a vector of a $\mathbb{CD}$ (In other words, functions operating on vectors)

$$
T: \mathbb{R}^n \to \mathbb{R}^m;\, T(\vec{v_1}) = \vec{v_2}
$$

## Linear transformations

A transformation is said to be linear if it follows both the **additive property** and the **homogeneous property**

$$
\text{Additive property}
$$
$$
T\left(\vec{a}+\vec{b}\right) = T\left(\vec{a}\right)+T\left(\vec{b}\right)
$$
$$
\text{Homogeneous property}
$$
$$
T\left(c \cdot \vec{a}\right) = c \cdot T\left(\vec{a}\right);\, \forall c \in \mathbb{R}
$$

Linear transformations have some properties that are listed below:

$$
T \text{ Is a linear transformation } \implies T\left(\vec{0}\right) = \vec{0}
$$
$$
T \text{ Is a linear transformation } \implies \text{ $T$ can be represented by a transformation matrix $A$} 
$$

**_Note_:** $A \iff A \cdot \vec{v} = T\left(\vec{v}\right)$

## Null space

The null space is the set of vectors that when transformed, equal the null vector;

$$
N(T) = \left\{\vec{v};\, T\left(\vec{v}\right) = \vec{0}\right\}
$$

## Eigenvalues and eigenvectors

$$
\vec{a} \text{ is an eigenvector of } A \iff A \cdot \vec{a} = \lambda \cdot \vec{a}
$$
$$
\lambda \text{ is an eigenvalue of } A \iff (A \cdot \vec{v}), \vec{v} \in \text{span}(\vec{v})
$$

### Determining the matrix of eigenvalues of a matrix

####  Using determinants

$$
\det(A - \lambda \cdot I) = 0
$$
$$
\Lambda=
\begin{bmatrix}
    \lambda_1 & 0 & 0 & ...\\
    0 & \lambda_2 & 0 & ...\\
    0 & 0 & \lambda_3 & ...\\
    ... & ... & ... & ...\\
\end{bmatrix}
$$

#### Using the matrix of eigenvectors

$$
\Lambda = S^{-1} \cdot A \cdot S
$$

### Determining the eigenvectors using the eigenspace

$$
E_{\lambda_n} = N(A - \lambda _n \cdot I)
$$

Determining the eigenspaces for all $\lambda$ values, you will find all the eigenvectors for the matrix $A$. You can create a matrix of eigenvectors as noted below:

$$
S=\left[E_{\lambda_1}|E_{\lambda_2}|E_{\lambda_3}|...\right]
$$

### Determining the transformation matrix using eigenvalues and eigenvectors

$$
A = S \cdot \Lambda \cdot S^{-1}
$$