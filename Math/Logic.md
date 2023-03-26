---
header-includes:
    - \usepackage{tikz}
    - \usetikzlibrary{circuits.logic.US}
---

**Table of contents**

- [Propositions](#propositions)
  - [Types of propositions](#types-of-propositions)
- [Truth value](#truth-value)
  - [Truth table](#truth-table)
- [Logical connectives](#logical-connectives)
- [Logic circuits](#logic-circuits)
  - [Logic gates](#logic-gates)

# Propositions

Declarative statement that assume either values: $\text{True}$ or $\text{False}$;

## Types of propositions

- Simple: Has no logical connectives;
- Complex: Has logical connectives;

# Truth value

Associate boolean values to a proposition;

## Truth table

Represent possible truth values of a simple or complex composition, a complete truth table should show all the logic steps to get to the result;

**Ex.:** Truth table of $(\neg p \leftrightarrow q)$

$$
\begin{matrix}
p & q & \neg p & \neg p \leftrightarrow q \\
\text{True} & \text{True} & \text{False} & \text{False} \\
\text{True} & \text{False} & \text{False} & \text{True} \\
\text{False} & \text{True} & \text{True} & \text{True} \\
\text{False} & \text{False} & \text{True} & \text{False}
\end{matrix}
$$

# Logical connectives

| $p$            | $q$            | $p \wedge q$   | $p \lor q$      | $p \rightarrow q$ | $p \leftrightarrow q$ |
|----------------|----------------|----------------|-----------------|-------------------|-----------------------|
| $\text{True}$  | $\text{True}$  | $\text{True}$  | $\text{True}$   | $\text{True}$     | $\text{True}$         |
| $\text{True}$  | $\text{False}$ | $\text{False}$ | $\text{True}$   | $\text{False}$    | $\text{False}$        |
| $\text{False}$ | $\text{True}$  | $\text{False}$ | $\text{True}$   | $\text{True}$     | $\text{False}$        |
| $\text{False}$ | $\text{False}$ | $\text{False}$ | $\text{False}$  | $\text{True}$     | $\text{True}$         |

- Not $(\neg)$: If $V(p) = \text{False}$ returns $\text{True}$ and vice-versa; 
- And $(\wedge)$: Only returns $\text{True}$ if both propositions are $\text{True}$;
- Or $(\lor)$: Only returns $\text{False}$ if both propositions are $\text{False}$;
- If, then $(\rightarrow)$: Only returns $\text{False}$ if the first propositions is $\text{True}$ and the second proposition is $\text{False}$;
- If, and only if $(\leftrightarrow)$: Only returns $\text{True}$ if $V(p) = V(q)$;  

**_Note:_** Equivalency symbols: $(\equiv \text{ or } \iff)$;

# Logic circuits

A logic circuit is a chain of logic gates that take the output from one gate to another gate that receives it as an input;

## Logic gates

A logic gate is a building block of a logic circuit and it implements operations to boolean values;

$$
\text{Not}
$$
$$
\begin{tikzpicture}[circuit logic US, every circuit symbol/.style={thick}]
  % NOT gate
  \node [not gate] (not) at (0,0) {};
  \draw (not.input) -- ++(-0.5,0) node[left] {A};
  \draw (not.output) -- ++(0.5,0) node[right] {$\neg$A};
\end{tikzpicture}
$$
$$
\text{And}
$$
$$ 
\begin{tikzpicture}[circuit logic US, every circuit symbol/.style={thick}]
  % AND gate
  \node [and gate,inputs={nn}] (and) at (0,0) {};
  \draw (and.input 1) -- ++(-0.5,0) node[left] {A};
  \draw (and.input 2) -- ++(-0.5,0) node[left] {B};
  \draw (and.output) -- ++(0.5,0) node[right] {A $\land$ B};
\end{tikzpicture}
$$  
$$
\text{Or}
$$
$$
\begin{tikzpicture}[circuit logic US, every circuit symbol/.style={thick}]
  % OR gate
  \node [or gate,inputs={nn}] (or) at (0,0) {};
  \draw (or.input 1) -- ++(-0.5,0) node[left] {A};
  \draw (or.input 2) -- ++(-0.5,0) node[left] {B};
  \draw (or.output) -- ++(0.5,0) node[right] {A $\lor$ B};
\end{tikzpicture}
$$
