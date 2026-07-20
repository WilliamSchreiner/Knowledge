Java é uma linguagem de programação orientada a objetos ([[POO]]) criada em 1995. Um dos seus principais objetivos é permitir que uma aplicação possa ser executada em diferentes sistemas operacionais, desde que exista uma Máquina Virtual Java (JVM) disponível.

---

#### Ambiente Java

##### JVM (Java Virtual Machine)

A **JVM** é a Máquina Virtual Java. Ela é responsável por executar o [[Binary Code]] gerado durante a compilação do programa, permitindo que uma mesma aplicação seja executada em diferentes plataformas sem precisar ser recompilada.

##### JRE (Java Runtime Environment)

A **JRE** é o ambiente de execução do Java. Ela contém a JVM e as bibliotecas necessárias para executar aplicações Java, mas não possui ferramentas para desenvolvimento, como o compilador.

Em outras palavras, a JRE é utilizada apenas para executar programas Java.

##### JDK (Java Development Kit)

O **JDK** é o kit de desenvolvimento do Java. Ele inclui tudo o que existe na JRE, além de ferramentas voltadas ao desenvolvimento, como o compilador (javac), depuradores e outras utilidades.

Sempre que eu for desenvolver aplicações Java, preciso utilizar o JDK.

---

#### Edições do Java

- **Java SE (Standard Edition):** versão base da plataforma Java, utilizada para o desenvolvimento de aplicações de uso geral.
    
- **Java EE (Enterprise Edition):** construída sobre o Java SE, adiciona recursos voltados ao desenvolvimento de aplicações corporativas e distribuídas.
    
- **Java ME (Micro Edition):** destinada ao desenvolvimento para dispositivos móveis e sistemas embarcados.
    
- **JavaFX:** conjunto de bibliotecas utilizado para desenvolver aplicações desktop com interfaces gráficas mais modernas.
    

---

#### Ecossistema Spring

Além da linguagem Java, existe o **Spring**, que é um dos principais ecossistemas para o desenvolvimento de aplicações.

Pelo que entendi, o Spring automatiza diversas tarefas que antes precisavam ser implementadas manualmente, como configuração de componentes, gerenciamento do ciclo de vida dos objetos e tratamento de requisições.

O framework utiliza anotações (metadados), como:

- @Component
- @Service
- @Controller
- @Repository

A partir dessas anotações, o Spring identifica cada componente da aplicação e realiza automaticamente a criação e a injeção das dependências necessárias para o seu funcionamento (Injeção de Dependência).

Outro recurso importante é a possibilidade de configurar propriedades da aplicação em arquivos externos, como informações de conexão com banco de dados, portas da aplicação e outras configurações, facilitando a manutenção e a alteração do ambiente sem modificar o código-fonte.

Mais detalhes em [[Spring]].

#### Referência

- Java. **O que é Java?** Disponível em: [https://www.java.com/pt-br/download/help/whatis_java.html](https://www.java.com/pt-br/download/help/whatis_java.html)