
## O que é ? 

O Apache Hadoop é uma plataforma de software de código aberto baseada em [[Java]] que gerencia o processamento e o armazenamento de dados para aplicações de big data. A plataforma funciona distribuindo jobs de big data e análise do Hadoop entre nós em um cluster de compute, dividindo-os em workloads menores que podem ser executados em paralelo. Alguns dos principais benefícios do Hadoop são escalabilidade, resiliência e flexibilidade. O Hadoop Distributed File System (HDFS) oferece confiabilidade e resiliência ao replicar qualquer nó do cluster para os outros nós do cluster, protegendo contra falhas de hardware ou software. A flexibilidade do Hadoop permite armazenar qualquer formato de dados, incluindo dados estruturados e não estruturados.

No entanto, as arquiteturas Hadoop apresentam uma série de desafios, principalmente com o passar do tempo. O Hadoop pode ser excessivamente complexo e exigir recursos e expertise significativos para configuração, manutenção e atualizações. Também é demorado e ineficiente devido às leituras e gravações frequentes usadas para realizar cálculos. A viabilidade de longo prazo do Hadoop continua a se degradar à medida que os principais provedores Hadoop começam a se afastar da plataforma, e também porque a necessidade acelerada de digitalizar incentivou muitas empresas a reavaliarem seu relacionamento com o Hadoop. 

> OBS: Tecnologia mais antiga, não é mais tão usada. E foi substituída por opções mais modernas como Spark
## O que é a programação Hadoop?

No framework Hadoop, o código é escrito principalmente em Java, mas parte do código nativo é baseada em C. Além disso, os utilitários de linha de comando são normalmente escritos como scripts de shell. Para o Hadoop MapReduce, o Java é usado com mais frequência, mas por meio de um módulo como o Hadoop streaming, os usuários podem usar a linguagem de programação de sua escolha para implementar o mapa e reduzir as funções.

## Como funciona ?

O Hadoop é um framework que permite a distribuição de conjuntos de dados gigantes em um cluster de hardware comum. O processamento Hadoop é realizado em paralelo em vários servidores simultaneamente.

Os clientes enviam dados e programas para o Hadoop. Em termos simples, o HDFS (um componente central do Hadoop) lida com os metadados e o sistema de arquivos distribuídos. Em seguida, o Hadoop MapReduce processa e converte os dados de entrada/saída. Por último, o YARN divide as tarefas no cluster.

Com o Hadoop, os clientes podem esperar um uso muito mais eficiente dos recursos de commodities com alta disponibilidade e um ponto de detecção integrado de falhas. Além disso, os clientes podem esperar tempos de resposta rápidos ao realizar consultas com sistemas de negócios conectados.

No geral, o Hadoop fornece uma solução relativamente fácil para organizações que buscam aproveitar ao máximo o big data.

Databricks; **What is hadoop**; Disponivel em:https://www.databricks.com/br/blog/what-is-hadoop