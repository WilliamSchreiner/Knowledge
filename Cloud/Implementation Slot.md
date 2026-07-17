
Os **Slots de Implantação** do Azure Functions permitem que uma mesma aplicação possua diferentes ambientes de execução, chamados de **slots**.

Cada slot representa uma instância separada da aplicação e possui seu próprio ponto de extremidade. O slot principal é o de **produção**, mas posso criar outros slots para validar novas versões antes de disponibilizá-las aos usuários.

Quando uma nova versão estiver pronta, é possível realizar a troca (**swap**) entre o slot de produção e outro slot, reduzindo o tempo de indisponibilidade e diminuindo os riscos durante a implantação.

A quantidade de slots disponíveis depende do plano de hospedagem utilizado no [[Serviço de aplicativo]].

> **Minha interpretação:** gosto de pensar nos slots como ambientes separados para a mesma aplicação. Embora não sejam contêineres, eles funcionam de forma parecida no sentido de permitir que versões diferentes coexistam até o momento da troca. Isso facilita a aplicação de estratégias de implantação sem afetar imediatamente os usuários.

## Utilização

Os Deployment Slots são bastante úteis para implementar estratégias de implantação, como:

- **[[Blue-Green Deployment]]**: manter duas versões da aplicação e alternar entre elas quando a nova versão estiver validada.
- **[[Canary Deployment]]**: liberar uma nova versão para uma pequena parcela dos usuários antes da disponibilização completa.
- **[[Staged Deployment]]**: validar alterações em um ambiente semelhante ao de produção antes de realizar a troca definitiva.

## Referências

Microsoft Learn. **Slots de implantação do Azure Functions**. Disponível em: [https://learn.microsoft.com/pt-br/azure/azure-functions/functions-deployment-slots?tabs=azure-portal](https://learn.microsoft.com/pt-br/azure/azure-functions/functions-deployment-slots?tabs=azure-portal)