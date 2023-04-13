### Teste – Treinamento Angular

## Introdução
Neste teste você irá desenvolver uma aplicação front-end utilizando o framework Angular para construir uma aplicação seguindo as seguintes diretrizes abaixo. Para fins didáticos e de correção objetiva iremos dividir o desenvolvimento do projeto em 4 etapas destacando a pontuação e critérios de correção. Para cada item destacado a seguir serão observados a corretude, mas também a qualidade do código produzido, especialmente o uso correto das construções e convenções do framework visando baixo acoplamento e alta coesão.

## Etapa 1 – Listagem de clientes (pontuação: 3)
Você deve consumir os dados da API GET /clientes e exibir na tela em forma de tabela, segue o componente para referência: https://getbootstrap.com/docs/5.3/content/tables

## Etapa 2 – Cadastro/atualização de clientes (pontuação: 4)
Você deverá utilizar os componentes de referência: https://getbootstrap.com/docs/5.3/forms/form-control
Você deve enviar os dados da API para:
Cadastro: POST /clientes (pontuação: 2)
Atualização: PUT /clientes (pontuação: 2)
Na tabela da tela de listagem de clientes, adicione uma coluna chamada “Ações” com o botão de Edição. Você deverá criar um service para clientes, diferenciando cadastro de atualização. Para a tela de atualização, você deverá passar o CPF pela URL ao clicar no botão de “Edição” da tela de listagem de clientes. No ngOnInit da tela de Edição, realize um GET /clientes/53210216002 passando o CPF, preenchendo os respectivos campos da tela.

## Etapa 3 – Remoção de clientes (pontuação: 3)
Na tabela da tela de listagem de clientes, adicione um novo botão Remover a coluna de “Ações”. Esse botão deverá ter uma confirmação e após a confirmação chamar DELETE /clientes/53210216002 passando o CPF como parâmetro.
