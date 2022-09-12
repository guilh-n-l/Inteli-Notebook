# Componentes
- Fita (Unidimensional e infinita): Armazena valores de entrada e saída;
- Unidade de controle: Explicita o estado atual da máquina, aponta para uma única célula da fita e realiza a leitura e a gravação de valores nessa. Além disso, ela deve ter a habilidade de se mover no eixo horizontal, mudando o estado da máquina;
- Programa: Sequência de ações determinadas em estados que devem executadas pela máquina;
<p align="center">
  <img width=60% src="https://i.imgur.com/sK2iW7z.png">
</p>
> OBS.: Segundo Hopcraft, Motwani e Ullman, uma máquina de turing pode ser definido como uma tupla de 7 elementos:

$\large{M = \{Q, \Sigma, \Gamma, \delta, q_0, B, F\} }$
- $Q$ = Conjunto de estados da máquina (finito);
- $\Sigma$ = Alfabeto de entrada (Não pode conter símbolos em branco);
- $\Gamma$ = Conjunto de símbolos da fita ($\Sigma \subset \Gamma$ e $null \in \Gamma$);
- $\delta$ = Função de posição;
- $q_0$ = Estado inicial da máquina;
- $B$ = Conjunto do símbolo nulo ($null$);
- $F$ = Conjunto de estados finais;

O programa vai definir, em estados, ações que devem ser realizadas. Essas ações dependem dos símbolos da fita, que podem ser modificados pela máquina. O estado final da fita determina o valor de saída;
<p align="center">
  <img width=90% src="https://i.imgur.com/N5ez5KD.png">
</p>

