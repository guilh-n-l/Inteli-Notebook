**Table of Contents**

- [Finding approximate root of a function using numerical values](#finding-approximate-root-of-a-function-using-numerical-values)
  - [Using the Newton method](#using-the-newton-method)
- [Numerical integration (Quadrature)](#numerical-integration-quadrature)
  - [Definite integrals using the Newton-Cotes method](#definite-integrals-using-the-newton-cotes-method)


# Finding approximate root of a function using numerical values

Using the intermediate value theorem (listed below), there are numerical methods to find the root between an interval $(a, b)$;


$$
\text{Intermediate value theorem:}
$$
$$
f(a) > 0 \, \And \, f(b) < 0 \implies \exists \, x_k \,;\, a<x_k<b \, \And \, f(x) \text{ is continuous}
$$

## Using the Newton method

$$
x_{n+1} = x_{n} - \frac{f(x_{n})}{f'(x_{n})} \, ; \, f'(x) = \frac{d}{dx}f(x) 
$$

# Numerical integration (Quadrature)

By using numerical techniques, you can approximate the computation of integral values;

## Definite integrals using the Newton-Cotes method

$$
\int_{a}^{b}f(x) \approx (b-a)\cdot \sum_{i=0}^{n} f(S_i) \cdot w_i
$$
$$
\small{
  S_i = \left\{\frac{(b-a) \cdot (i+1)}{n}, ... \right\}
}
$$
$$
\begin{array}{cc|ccccc}
  n & \text{Factor} &&& \frac{w_i}{\text{Factor}}&&\\
  \\
  1 & \frac{1}{2} & 1 & 1 &&&\\
  \\
  2 & \frac{1}{6} & 1 & 4 & 1 &&\\
  \\
  3 & \frac{1}{8} & 1 & 3 & 3 & 1 &\\
  \\
  4 & \frac{1}{90} & 7 & 32 & 12 & 32 & 7\\
\end{array}
$$

Ex.:

$$
\text{Solve the definite integral below using the Newton-Cotes method of order 4}
$$
$$
\int_1^5 \sqrt[3]{x}
$$
Resolution:
$$
S_i = \left\{\frac{4 \cdot 1}{4}, \frac{4 \cdot 2}{4}, \frac{4 \cdot 3}{4}, \frac{4 \cdot 4}{4}, \frac{4 \cdot 5}{4}\right\} = \left\{1, 2, 3, 4, 5\right\}
$$
$$
\int_1^5 \sqrt[3]{x} \approx (5-1) \sum_{i=0}^{4} \sqrt[3]{S_i} \cdot w_i = 4 \cdot \left(\left(\sqrt[3]{1}\cdot \frac{7}{90}\right) + \left(\sqrt[3]{2}\cdot \frac{32}{90}\right) + \left(\sqrt[3]{3}\cdot \frac{12}{90}\right) + \left(\sqrt[3]{4}\cdot \frac{32}{90}\right) + \left(\sqrt[3]{5}\cdot \frac{7}{90}\right) \right) \approx 5.6618 
$$