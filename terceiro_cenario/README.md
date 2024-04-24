# 3º Cenário:
O cliente entrou em contato devido a uma questão relacionada aos seus anúncios. Quando os itens ficam sem estoque, em vez de serem marcados como "Pausado (sem estoque)", eles estão apenas sendo marcados como "Pausado", o que faz com que os anúncios permaneçam disponíveis para venda no Mercado Livre, mesmo sem estoque real. Isso está resultando em pedidos sendo feitos para itens sem estoque disponível, o que prejudica a reputação do cliente, pois ele precisa cancelar as vendas devido à falta de estoque.

Atualmente, o cliente possui 38 anúncios com a situação "Pausado", e ele relata que não os marcou manualmente como pausados. Quando enviamos uma atualização manual de estoque, o anúncio muda para a situação "Pausado sem estoque" e fica indisponível para venda no Mercado Livre. Ao verificar o log dos anúncios, não encontramos registros de envio de informação de estoque igual a zero quando o estoque se esgota no Magazord. Um exemplo de anúncio afetado é o seguinte: MLB3097510082. Envio em anexo um print do anúncio e um print do log, mostrando que não foram encontradas informações registradas na abertura da atividade.

---
Para o caso acima, descreva quais seriam os passos para analise e identificação do problema tendo em vista a documentação do próprio ML. Visto que não possui acesso ao painel seller do cliente e nem ao painel do mesmo no ERP Magazord, quais seriam as possíveis hipóteses do erro.

![Imagem anúncio](/img/1.cen3_anuncio.png)