- [Partial derivatives](#partial-derivatives)
  - [Notation](#notation)
  - [Chain rule](#chain-rule)

# Partial derivatives

To solve partial derivatives, hold the other variables (The ones other variables than the one you are deriving from) constant, then solve the derivative as a total one;

Ex.:

$$
\frac{\partial}{\partial x} 2x^2 + xy + z
$$
$$
\text{Factoring out the highest power from each monomial}
$$
$$
\frac{\partial}{\partial x} 2x^2 + xy + z=
$$
$$
4x + y
$$

## Notation

$$
\frac{\partial f}{\partial x} = f_x
$$
$$
\frac{\partial^2 f}{\partial x^2} = \frac{\partial}{\partial x} \frac{\partial f}{\partial x} = f_{xx}
$$
$$
\frac{\partial^2 f}{\partial xy} = \frac{\partial}{\partial x} \frac{\partial f}{\partial y} = f_{xy}
$$

## Chain rule

To solve partial derivatives where the variable you are deriving from is dependent on other variables $\left(x(t)\right)$, one can use the chain rule;

$$
\frac{dz}{dt} = \frac{\partial z}{\partial x}\cdot\frac{dx}{dt}+\frac{\partial z}{\partial y}\cdot\frac{dy}{dt}; y=f(t) \, \And \, x=g(t)
$$