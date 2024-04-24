# Testar campo `Nome Completo`
> Objetivo: verificar o funcionamento do campo `Nome Completo` na rotina de Cadastro de cliente

1. Acessar Consultar Pessoas >> Selecionar um usuário >> Alterar 
2. No campo nome, inserir o texto 'NomeSobrenome' >> Confirmar
  - Não deve permitir, tendo em vista que configura apenas nome
3. No campo nome, inserir 'Nome Sobrenome123#%&'
  - Não deve permitir iserir o conteúdo alfanumérico
4. No campo nome, inserir 'Nome Sobrenome' >> Confirmar
  - Deve alterar corretamente

# Testar campo `E-mail`
> Objetivo: verificar o funcionamento do campo `E-mail` na rotina de Cadastro de cliente

1. Acessar Consultar Pessoas >> Selecionar um usuário >> Alterar
2. No campo e-mail, inserir o texto 'testemagazord.com.br' >> Confirmar
  - Não deve permitir, pois não possui o '@', ou seja, não é um e-mail válido
3. No campo e-mail, inserir o texto '$%'
  - Não deve permitir, pois o e-mail não permite esse tipo de caracter
4. No campo e-mail, inserir '@magazord.com.br'>> Confirmar
  - Não deve permitir, pois não contém um e-mail válido
5. No campo e-mail, inserir 'teste@magazor.com.br' >> Confirmar
  - Deve alterar corretamente

# Testar campo `Número de telefone`
> Objetivo: verificar o funcionamento do campo `Número de Telefone` na rotina de Cadastro de cliente

1. Acessar Consultar Pessoas >> Selecionar um usuário >> Alterar
2. No campo número, informar o texto 'asdf@#$'
  - Não deve permitir inserir, pois não é conteúdo numérico
3. No campo número, informar texto '991039519' >> Confirmar
  - Deve informar que o número está incorreto
4. No campo número, informar texto '47991039519' >> Confirmar
  - Deve formatar corretamente e permitir a inserção
5. No campo número, informar texto '(47) 99103-9519' >> Confirmar
  - Deve permitir, sendo um número válido

# Testar campo `Data de Nascimento`
> Objetivo: verificar o funcionamento do campo `Data de Nascimento` na rotina de Cadastro de cliente

1. Acessar Consultar Pessoas >> Selecionar um usuário >> Alterar
2. No campo data de nascimento, informar o texto 'asdf!@#'
  - Não deve inserir o texto
3. No campo data de nascimento, informar o texto '070104' >> Confirmar
  - Não deve permitir, pois não é uma data completa
4. No campo data de nascimento, informar o texto '07012004' >> Confirmar
  - Deve formatar corretamente e permitir o cadasto
5. No campo data de nascimento, informar o texto '07/01/2004' >> Confirmar
  - Deve permitir
6. No campo data de nascimento, selecionar uma data através do ícone de calendário
  - Deve permitir e armazenar a seleção corretamente

# Testar campo `Endereço`
> Objetivo: verificar o funcionamento dos campos do grupo `Endereço` na rotina de Cadastro de cliente

1. Acessar Consultar Pessoas >> Selecionar um usuário >> Alterar
2. No campo CEP, informar o texto 'as!@#$'
  - Não deve permitir
3. No campo CEP, informar um CEP qualquer (utilizar <https://www.4devs.com.br/gerador_de_cep>, se necessário)
  - Ao tirar o foco do campo, deve buscar os demais dados do endereço corretamente
4. Preencher os campos Rua, Cidade e Estado
  - Deve preencher o campo CEP
