# Sistema Binário

O sistema de numeração binária é um dos diversos sistemas numéricos utilizados atualmente. Enquanto o sistema decimal utiliza a base 10, o sistema binário utiliza a base 2, ou seja, trabalha apenas com dois valores possíveis: 0 e 1.

Pelo que estudei, o sistema binário foi aperfeiçoado no século XVII pelo matemático alemão Gottfried Leibniz, que apresentou seus fundamentos na obra _Explicação da Aritmética Binária_, publicada em 1703.

Cada dígito binário é chamado de bit (_binary digit_). Um bit pode assumir apenas dois valores:

- **0** > desligado;
- **1** > ligado.

Esses dois estados são a base do funcionamento dos computadores.

---

# Como o computador utiliza o sistema binário

Os computadores representam todas as informações utilizando sequências de 0 e 1. Internamente, esses valores correspondem a sinais elétricos presentes nos transistores da [[CPU]] e da [[Memória RAM]].

De forma simplificada:

- **1** representa a presença de um sinal elétrico (ligado);
- **0** representa a ausência desse sinal (desligado).

A partir dessas combinações de bits, o computador consegue representar números, textos, imagens, sons e qualquer outro tipo de dado digital.

---

# Como funcionam os números binários

O sistema binário é a linguagem utilizada pelos computadores para representar informações.

Normalmente, um conjunto de 8 bits forma um byte. Cada posição dentro desse byte possui um valor específico, que aumenta em potências de dois da direita para a esquerda.

| Posição do bit |   8 |   7 |   6 |   5 |   4 |   3 |   2 |   1 |
| -------------- | --: | --: | --: | --: | --: | --: | --: | --: |
| Potência de 2  |  2⁷ |  2⁶ |  2⁵ |  2⁴ |  2³ |  2² |  2¹ |  2⁰ |
| Valor decimal  | 128 |  64 |  32 |  16 |   8 |   4 |   2 |   1 |

Sempre que um bit possuir valor **1**, o valor correspondente daquela posição será somado. Quando o bit for 0, aquele valor é ignorado.

---

# Exemplo

Considere o número binário:

```text
00110110
```

Distribuindo os bits nas posições:

|Posição|8|7|6|5|4|3|2|1|
|---|--:|--:|--:|--:|--:|--:|--:|--:|
|Bit|0|0|1|1|0|1|1|0|
|Valor|128|64|32|16|8|4|2|1|

Somente os bits iguais a 1 participam da soma:

- 32
- 16
- 4
- 2

Resultado:

```text
32 + 16 + 4 + 2 = 54
```

Portanto,

```text
00110110₂ = 54₁₀
```

> Minha interpretação: converter um número binário para decimal consiste apenas em identificar quais posições possuem valor **1** e somar os respectivos valores das potências de dois.

---

# Referência

- TechTarget. **O que é binário e como ele é usado na computação?** Disponível em: [https://www.techtarget.com/whatis/definition/binary](https://www.techtarget.com/whatis/definition/binary)