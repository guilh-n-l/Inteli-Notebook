# Classes & Objetos
- Classe: Agrupamento de objetos (molde) de mesma natureza, ainda que eles possuam características diferentes;
- Objeto: Entidades de ocorrência específica de uma classe. Tem características próprias provenientes de classe que o originou;

> OBS.: A criação de um objeto a partir de uma classe é chamada de instanciação de classe;

Ex.:
```Python
class Carro:
Corrola = Carro()
```

# Conceitos importantes
- **Métodos** são as ações que um objeto pode realizar;
- **Atributos** são propriedades de um objeto;
 - Estáticos: Carregam o mesmo valor durante toda a sua existência;
 - Dinâmicos: Seus valores podem variar com o passar do tempo;
- **Mensagens** são a forma como os objetos se comunicam entre si se estiverem ligados por alguma associação
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

# Criando uma classe
```Python
class Dog:
def __init__(self, dogBreed, dogEyeColor, dogMood):
	self.breed = dogBreed
	self.eyeColor = dogEyeColor
	self.mood = dogMood
Scoot = Dog("Cavalier King Charles", "Brown", "Sleepy")
```
- `__init__` é o método construtor que define os atributos presentes em todos os objetos da classe. Ele sempre começa com o `self` que junta os atributos dos objetos aos argumentos recebidos;