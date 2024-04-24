# Execução dos Teste

## Ambiente de teste
- Inicialmente os testes devem ser executados em ambiente staging, de forma a não impactar outros testes e, principalmente, a base de produção.
- Passados os testes em ambiente `staging`, os mesmos devem ser executados em base de `homologação`, para que os arquivos desenvolvidos sejam testados em conjunto com outros.
- Em sequência, devem ser executados testes em base `production`, sendo uma última simulação antes de liberar para a base de produção.

## Dados de testes
- Podem ser utilizados dados gerados em ambientes de qualidade (staging e homologação), buscando cadastrar dados semelhantes aos do cliente.
- Pode ser realizado um backup periódico da base do cliente para ser utlizado em base de qualidade.

## Ferramentas de teste
- Testes de API: Postman, preferencialmente, ou SoapUi.
- Testes de automação: Selenium.
- Testes de carga: JMeter.

## Registro de resultados
 - Uso de planilha (Excel ou Google Sheets) para registro de dados e resultados de testes, bem como elaboração de gráficos de desempenho, etc.
 - Jira ou Trello para acompanhamento e mapeamento dos testes.