**Table of contents**

- [Vectors](#vectors)
  - [Parametric representation of lines](#parametric-representation-of-lines)
  - [Linear combination](#linear-combination)
    - [Span](#span)
  - [Linear independence](#linear-independence)
  - [Vector transformations](#vector-transformations)
    - [Introduction to transformations: Multi-variable functions](#introduction-to-transformations-multi-variable-functions)

# Vectors 

## Parametric representation of lines

A line in an $n$ dimensional space can be represented using a vector equation, such as the one below:

$$
S = \{k \cdot \vec{v};\, k \in \mathbb{R}\}
$$

## Linear combination

Given a set of vectors and a set of scalars, a linear combination is a combination of those two sets

$$
V = \{\vec{v_1}, \vec{v_2}, \vec{v_3}, ...;\, \forall \vec{v_i} \in \mathbb{R^n}\}
\,\And\,
C = \{c_1, c_2, c_3, ...;\, \forall c_i \in \mathbb{R}\}
$$
$$
c_1 \cdot \vec{v_1} + c_2 \cdot \vec{v_2} + ... \rightarrow \text{ one linear combination of $C$ and $V$}
$$

### Span

The span of a set of vectors $\left(\text{Span}\left(\vec{v_1}, \vec{v_2}, \vec{v_3}, ...\right)\right)$ is the set of all possible linear combinations between that set of vectors and the set of real numbers;

## Linear independence

When a set of vectors can't represent all of it's vectors using linear combination of all the other vectors in the set, it is said that this set is linearly independent;

$$
c_1 \cdot \vec{v_1} + c_2 \cdot \vec{v_2} + ... = \vec{0}
\implies
\begin{cases}
  \text{Linearly independent};\,\nexists\, c_i \ne 0\\
  \text{Linearly dependent};\,\exists\, c_i \ne 0\\
\end{cases}
$$



## Vector transformations

### Introduction to transformations: Multi-variable functions 

$$
f(x, y, ...) = z
$$

$$
\mathbb{D} = \mathbb{R}^n \,\And\, \mathbb{CD} = \mathbb{R}
$$