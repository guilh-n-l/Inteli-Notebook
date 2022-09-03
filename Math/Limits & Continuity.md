# Funções contínuas
- Uma função é considerada contínua em um ponto **(p)** quando nesse ponto não existe um "salto" no valor em **f(p)**, ou seja, a medida em que **x** de aproxima de **p**, mais próximo **f(x)** estará de **f(p)**;
<p align="center">
  <img width=60% src="https://i.imgur.com/Zm5zpFA.png">
  <figcaption><p align="center">Função contínua</figcaption>
</p>
<p align="center">
  <img width=60% src="https://i.imgur.com/rD9Nw7r.png">
  <figcaption><p align="center">Função descontínua</figcaption>
</p>

# Limite
- Seja **f** uma função e **a** um ponto no domínio de **f**, dizemos que o limite **L** de **f** no ponto **a** é a imagem do ponto infinitamente próximo a **a**;

Ex.: Na função abaixo($f(x) = \frac{1}{x}$), na medida em que x se aproxima de 0, a imagem se torna mais próxima de $+\infty$ pela direita e $-\infty$ pela esquerda
<p align="center">
  <img width=80% src="https://i.imgur.com/IgeFyLC.png">
  <figcaption><p align="center"></figcaption>
</p>
## Limites laterais
> Limites laterais são utilizados para explicitar um limite divergente

Ex.: $\lim_{x \to 0^+}{\frac{1}{x}} = +\infty$ == O limite de $\frac{1}{x}$ pela direita quando $x$ tende à zero é $+\infty$;
Ex.: $\lim_{x \to 0^-}{\frac{1}{x}} = +\infty$ == O limite de $\frac{1}{x}$ pela esquerda quando $x$ tende à zero é $-\infty$;

> OBS.: Quando os **limites laterais** de uma função pela esquerda e pela direita em um ponto **existirem** porém terem valores diferentes, pode-se dizer então que o **limite dessa função** nesse ponto **não existe**;

## Teorema do confronto (Squeeze Theorem)
1. Suponha a existência de 3 funções: $f(x), g(x), h(x)$
2. Considere $f(x)\leq g(x)\leq h(x)$
3. Se $lim_{x \to p}{f(x)} = lim_{x \to p}{h(x)} = L \implies lim_{x \to p}{g(x)} = L$
  