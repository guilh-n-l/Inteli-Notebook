**Table of Contents**

- [Indefinite integrals](#indefinite-integrals)
- [Integration](#integration)
  - [Definite integrals](#definite-integrals)
    - [Primitive method](#primitive-method)
    - [Sum of Riemann method](#sum-of-riemann-method)



# Derivatives

$$
(f \cdot g)' = f'g + fg' 
$$

$$
\left(\frac{f}{g}\right)' = \frac{f'g - fg'}{g^2}
$$

$$
\frac{df}{dx} = \frac{df}{du} \cdot \frac{du}{dx}
$$

# Integration

## Definite integrals

### Primitive method

$$
\int_a^bf(x)\,dx = F(b)-F(a)\,; \frac{d}{dx}F(x) = f(x)
$$

**_Note:_** $F(x)$ is called the **antiderivative** or **primitive** of $f(x)$;

### Sum of Riemann method

$$
\int_a^bf(x)\,dx = \lim_{n \to \infty}\sum_{i=1}^n\left(\frac{b-a}{n}\cdot f(x_i)\right)
$$