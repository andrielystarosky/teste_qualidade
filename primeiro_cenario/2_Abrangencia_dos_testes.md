# Abrangência dos testes

## Funcionalidades
- Devem ser testadas todas as funcionalidade previstas em contrato, conforme levantamento realizado durante análise. 
- Deve ser garantido o funcionamento esperado das integrações citadas: estoque, anúncios, faturamento, pedidos e preço.
- Devem ser realizados testes que garantam o funcionamento do usuário final enquanto a compra, devolução, cancelamento, cálculo de frete, cupons de desconto, etc.
- Devem ser simuladas, em primeira instância, testes que garantam usabilidades básicas, como inclusão/retirada de determinado produto, esgotamento de estoque, etc.

## Casos de uso
> Devem ser testados todos os possíveis cenários de uso de cada funcionalidade. Exemplos (condensados - sem passo a passo, pois depende do sistema/rotina):
- Estoque
  - Realizar uma compra de um produto sem estoque (falha)
  - Realizar compra do último produto em estoque (sucesso, informando esgotamento para o próximo usuário)
  - Compra de quatidade superior a um limite de aquisição previamente estipulado (falha)
  - Compra de quantidade superior ao disponível em estoque (falha)
  - Compra de um produto disponível (sucesso)
- Anúncios
  - Acessar un anúncio (sucesso)
  - Visualizar o carregamento (sucesso)
  - Opções de sair/pular anúncio
- Faturamento
  - Realizar uma venda no sistema (sucesso)
  - Avaliar a fatura emitida, contendo os dados previstos em regra de negócio (sucesso)
  - Avaliar a notificação enviada contendo faturamento (sucesso)
- Pedidos
  - Adicionar/remover produtos ao carrinho (sucesso).
  - Concluir/cancelar pedidos (sucesso).
  - Verificar confirmação de pedidos (sucesso).
  - Verificar notificação de pedido ao cliente e ao vendedor (sucesso).
- Preço
  - Verificar se o preço do anúncio é o mesmo do preço real do produto (sucesso).
  - Verificar aplicação de frete (sucesso).
  - Verificar aplicação de cupons de desconto (sucesso).

- Quanto a teste de carga, deve-se se simular uma quantidade grande de usuários executando diversas ações simultaneamente, bem como diversos usuários realizando a mesma ação. Isso afim de garantir estabilidade do serviço mesmo diante de uma quantidade de acessos não comum (como em dias promocionais, por exemplo).

## Priorização de testes
> A prioridade dos testes podem ser divididas em:
- Altíssima: são funcionalidades essenciais para o funcionamento do sistema (normalmente requisitos não funcionais; possivelmente erros que estão impedindo a realização de alguma rotina; questões relacionadas a segurança).
- Alta: são funcionalidades importantes para o sistema/usuário, mas não são vitais para tal (normalmente requisitos funcionais importantes para o funcionamento de rotinas essenciais).
- Média: são funcionalidades importantes, mas o sistema segue funcionando sem elas (normalmente melhorias ou questões relacionadas a usabilidade, questões com soluções paliativas).
- Baixa: são funcionalidades ou até mesmo melhorias não tão importantes, mas que aprimoram o sistema (normalmente melhorias internas, restritas a ambientes de qualidade e desenvolvimento).
