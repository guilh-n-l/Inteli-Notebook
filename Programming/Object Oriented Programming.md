# Classes & Objetos
- Classe: Agrupemento de objetos de mesma natureza, ainda que eles possuam características diferentes;
- Objeto: Agrupemento de objetos de mesma natureza, ainda que eles possuam características diferentes;

> OBS.: A criação de um objeto a partir de uma classe é chamada de instanciação de classe;

Ex.:
```Python
class Carro:
Corrola = Carro()
```

# Conceitos importantes
- **Métodos** são as ações que um objeto pode realizar;
- **Atributos** são propriedades de um objeto;
- Métodos e atributos são **públicos** quando são visíveis fora de um objeto. Caso o contrário, eles seram chamados de **privados**;

# Propriedades da POO
- Encapsulamento: Tornar métodos e atributos privados para que eles não possam ser modificados fora da classe;
- Herança: Uma classe pode herdar características de outra classe mãe;
<p align="center">
  <img width=80% src="https://i.imgur.com/s8RyLAq.png">
</p>
- Interface: 2+ classes possuem características em comum que podem ser separados em uma outra "classe" (Não é uma classe e sim um conjunto de métodos e atributos). Essa outra "classe" pode ser chamada de interface;
> OBS.: Uma interface não é herdada por outras classes, mas sim implementada nelas. Lembrando que ao implementar uma interface, todas as suas características são implementadas nas classes;
<p align="center">
  <img width=80% src="https://i.imgur.com/UnQ674B.png">
</p>
- Polimorfismo: Um método é considerado polimorfismo quando pode ser implementado de uma forma diferente em diferentes classes ou em diferentes objetos;
- Design patterns: Formas de resolver problemas comuns em linguagens orientadas a objetos;