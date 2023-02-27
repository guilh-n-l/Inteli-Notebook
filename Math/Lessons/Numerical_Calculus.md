**Table of Contents**

- [Finding approximate root of a function using numerical values](#finding-approximate-root-of-a-function-using-numerical-values)
  - [Using the Newton method](#using-the-newton-method)


# Finding approximate root of a function using numerical values

Using the intermediate value theorem (listed below), there are numerical methods to find the root between an interval $(a, b)$;


$$
\text{Intermediate value theorem:}
$$
$$
f(a) > 0 \, \And \, f(b) < 0 \implies \exist \, x_k \,;\, a<x_k<b \, \And \, f(x) \text{ is continuous}
$$

## Using the Newton method

$$
x_{n+1} = x_{n} - \frac{f(x_{n})}{f'(x_{n})} \, ; \, f'(x) = \frac{d}{dx}f(x) 
$$

