
Existem duas formas principais de aumentar ou reduzir a capacidade de uma aplicação: **escalabilidade horizontal** e **escalabilidade vertical**.

## Escala horizontal (Scaling Out)

A escala horizontal consiste em adicionar novas máquinas ou instâncias para distribuir a carga da aplicação. Em vez de aumentar os recursos de um único servidor, a capacidade é ampliada criando novas instâncias que trabalham em conjunto.

Para que isso funcione, é necessário um mecanismo responsável por distribuir as requisições entre as instâncias disponíveis, como um [[Load Balancer]]. Esse componente garante que a carga fique equilibrada e que cada requisição seja encaminhada para uma instância adequada.

Quando a demanda diminui, essas instâncias também podem ser removidas, processo conhecido como **Scaling In**.

### Exemplo

Se uma API estiver recebendo um número muito alto de requisições, em vez de aumentar a capacidade do servidor atual, posso criar novas instâncias da aplicação. Assim, as requisições passam a ser distribuídas entre todas elas, aumentando a capacidade de atendimento.

## Escala vertical (Scaling Up)

A escala vertical consiste em aumentar os recursos de uma única máquina. Em vez de adicionar novos servidores, são ampliados recursos como:

- CPU;
- Memória RAM;
- Armazenamento.

Da mesma forma, quando a demanda diminui, esses recursos podem ser reduzidos (Scaling Down).

### Exemplo

Imagine uma API hospedada em uma máquina virtual com:

- 1 núcleo de CPU;
- 512 MB de memória RAM.

Se essa aplicação precisar de mais desempenho, posso aumentar a máquina para:

- 2 núcleos de CPU;
- 1 GB de memória RAM.

Com mais recursos disponíveis, a expectativa é que a aplicação consiga processar um número maior de requisições. Entretanto, o ganho nem sempre é proporcional, pois fatores como largura de banda da rede, velocidade do armazenamento e outras limitações também influenciam no desempenho.

## Comparação

|Escala Horizontal|Escala Vertical|
|---|---|
|Adiciona novas máquinas ou instâncias.|Aumenta os recursos de uma única máquina.|
|Distribui a carga entre várias instâncias.|Toda a carga continua concentrada em um único servidor.|
|Geralmente utiliza um balanceador de carga.|Não necessita balanceamento de carga.|
|Possui maior disponibilidade e tolerância a falhas.|Continua sendo um único ponto de falha.|
|Normalmente é mais utilizada em aplicações na nuvem.|Possui limite físico dos recursos da máquina.|

> **Minha interpretação:** penso na escalabilidade horizontal como "adicionar mais caixas para atender os clientes", enquanto a escalabilidade vertical seria "aumentar o tamanho da única caixa que já existe". Em ambientes de nuvem, normalmente a escala horizontal é a abordagem mais utilizada, pois oferece maior disponibilidade e facilita o crescimento da aplicação.

### Imagem

![[Pasted image 20260623163003.png]]