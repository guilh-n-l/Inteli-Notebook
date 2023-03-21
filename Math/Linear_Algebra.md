**Table of contents**

- [Vectors](#vectors)
  - [Parametric representation of lines](#parametric-representation-of-lines)
  - [Linear combination](#linear-combination)
    - [Span](#span)
  - [Linear independence](#linear-independence)
  - [Subspace of a vector set](#subspace-of-a-vector-set)
  - [Vector transformations](#vector-transformations)

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

$$
\text{only if there is no solution for $(c_1 \cdot \vec{v_1} + c_2 \cdot \vec{v_2} + c_3 \cdot \vec{v_3} +... = 0)$ other than when $\forall c_i = 0$, that the set of vectors is linearly independent}
$$

## Subspace of a vector set

A subset $\mathbf{U}$ is said to be a subspace of a superset $\mathbf{V}$ when $\mathbf{U}$ follows all the condtions below:

$$
\begin{equation}
\vec{0} \in U
\end{equation}
$$
$$
\begin{equation}
\text{$\mathbf{U}$ contains all the linear combinations of vectors in itself (Is closed in vector addition)}
\end{equation}  
$$
$$
\begin{equation}
\text{$\mathbf{U}$ contains all the scalar products of vectors in itself (Is closed in scalar multiplication)}
\end{equation}  
$$

## Vector transformations

Vector transformations are the association between vectors from a $\mathbb{D}$ to a vector of a $\mathbb{CD}$ (In other words, functions operating on vectors)

$$
T: \mathbb{R}^n \to \mathbb{R}^m;\, T(\vec{v_1}) = \vec{v_2}
$$