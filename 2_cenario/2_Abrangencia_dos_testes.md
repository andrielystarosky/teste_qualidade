# Abrangência dos Testes

## Funcionalidades
 - Devem ser testadas todas as funcionalidade previstas em contrato, conforme levantamento realizado durante análise. 
  - Exemplos: sincronização de produtos, relatórios de venda, atualização de estoque, processamento de pedidos, categorias dos produtos. 
  - Devem ser simuladas, em primeira instância, testes que garantam usabilidades básicas, como inclusão/retirada de determinado produto, esgotamento de estoque, etc.

## Priorização de testes
> A prioridade dos testes pode ser dividida em:

| Nível de Prioridade | Definição |
| ---                 | ---       |
| Altíssima           | são funcionalidades essenciais para o funcionamento do sistema (normalmente requisitos não funcionais; possivelmente erros que estão impedindo a realização de alguma rotina; questões relacionadas a segurança) |
| Alta                | são funcionalidades importantes para o sistema/usuário, mas não são vitais para tal (normalmente requisitos funcionais importantes para o funcionamento de rotinas essenciais)|
| Média               | são funcionalidades importantes, mas o sistema segue funcionando sem elas (normalmente melhorias ou questões relacionadas a usabilidade, questões com soluções paliativas) |
| Baixa              | são funcionalidades ou até mesmo melhorias não tão importantes, mas que aprimoram o sistema (normalmente melhorias internas, restritas a ambientes de qualidade e desenvolvimento) |