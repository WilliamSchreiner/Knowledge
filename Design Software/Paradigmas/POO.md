
A Programação Orientada a Objetos (POO) é um paradigma de programação que organiza o código utilizando classes e objetos. A ideia é representar elementos do mundo real dentro do software, tornando o código mais organizado, reutilizável e fácil de manter.

Pelo que entendi, a POO busca dividir um sistema em pequenas unidades chamadas **objetos**, onde cada uma possui características (atributos) e comportamentos (métodos). A interação entre esses objetos é o que permite o funcionamento da aplicação.

---

# Classes

Antes de criar um objeto, é necessário definir uma **classe**.

Uma classe pode ser vista como um **molde** ou um **modelo**, que descreve como determinado tipo de objeto será criado. Nela são definidos os dados e os comportamentos que todos os objetos daquele tipo terão.

Dependendo da linguagem utilizada, uma classe pode conter:

- atributos ([[Propriedades]]);
- métodos ([[Funções]]);
- construtores([[Constructors]]);
- modificadores de acesso;
- outros elementos específicos da linguagem.
    
> **Minha interpretação:** gosto de pensar na classe como um projeto de uma casa. O projeto descreve como ela será construída, mas ainda não existe nenhuma casa de fato.

---

# Objetos

Um objeto é uma instância criada a partir de uma classe.

Quando um objeto é criado, ele passa a ocupar um espaço na memória e possui seus próprios valores para os atributos definidos pela classe. Mesmo que dois objetos sejam criados a partir da mesma classe, cada um pode armazenar informações diferentes.

> **Minha interpretação:** se a classe representa o projeto da casa, o objeto é a casa já construída. Posso utilizar o mesmo projeto para construir várias casas, mas cada uma terá seu próprio endereço, moradores e características.

---

# Relação entre classes e objetos

Em uma aplicação orientada a objetos, normalmente existem diversas classes representando diferentes partes do sistema.

Durante a execução do programa, essas classes são instanciadas, criando objetos que interagem entre si por meio de seus métodos. Essa comunicação é o que permite implementar as funcionalidades da aplicação.

---

# Exemplo

```java
public class Pessoa {

    String nome;
    int idade;

    void apresentar() {
        System.out.println("Olá, meu nome é " + nome);
    }
}
```

Criando um objeto dessa classe:

```java
Pessoa pessoa = new Pessoa();

pessoa.nome = "William";
pessoa.idade = 25;

pessoa.apresentar();
```

Nesse exemplo:

- Pessoa é a classe;
- pessoa é um objeto criado a partir da classe;
- nome e idade são os atributos;
- apresentar() é um método.

---

# Referência

- Alura. **POO: o que é programação orientada a objetos? Entenda o conceito e veja exemplos práticos.** Disponível em: [https://www.alura.com.br/artigos/poo-programacao-orientada-a-objetos?srsltid=AfmBOooP2av6NcHaFCqv58CAQwCvjNymVdKcjM1JFZsmi82hBexODzVv](https://www.alura.com.br/artigos/poo-programacao-orientada-a-objetos?srsltid=AfmBOooP2av6NcHaFCqv58CAQwCvjNymVdKcjM1JFZsmi82hBexODzVv)