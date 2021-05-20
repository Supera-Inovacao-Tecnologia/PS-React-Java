# Avaliação Java + React

## Descrição

O teste consiste em construir a camada de serviço de um pseudo e-commerce de games utilizando Java, e consumir este serviço atavés de uma API HTTP para construir a interface do e-commerce utilizando React Web.

## Como executar os testes
  
O projeto usa o maven wrapper (mvnw).
Para executar os testes de exemplo basta o comando abaixo:
```sh
./mvnw clean test
```

## Requisitos Funcionais

- Existe um exemplo de carga de banco de dados em memória em [ProductDaoExampleTest.java](./src/test/java/br/com/supera/game/store/ProductDaoExampleTest.java) que possui uma lista de produtos que devem ser renderizados dinamicamente.
- As imagens que devem ser utilizadas também estão inclusas na pasta [assets](./assets).
- O usuário poderá adicionar e remover produtos do carrinho.
- O usuário poderá ordenar os produtos por preço, popularidade (score) e ordem alfabética. A filtragem deve ser realizada pela API.
- Os valores exibidos no checkout (frete, subtotal e total) devem ser calculados dinamicamente conforme o usuário seleciona ou remove produtos.
- A cada produto adicionado, deve-se somar R$ 10,00 ao frete.
- Quando o valor dos produtos adicionados ao carrinho for igual ou superior a R$ 250,00, o frete é grátis.
- O usuário pode realizar checkout de seu carrinho de compras. Deve ser exigido preencher informações pessoais do usuário (Nome, CPF, Endereço, Número do Cartão de Crédito). A API deverá validar se as informações pessoais foram preenchidas e o preço a ser pago conforme os requisitos anteriores. As informações deverão ser inseridas no banco de dados em memória.

## Requisitos Não Funcionais

- Deverá ser documentado no [README.md](./README.md) como executar/compilar/empacotar o projeto e quais os endpoints solicitados nos requisitos acima. Para esse fim podem ser utilizadas ferramentas de containerização e automatização de builds.
- A API deverá ser HTTP e pode ser REST ou GraphQL.
- A versão do Java deve ser 11 ou superior.
- Não existe restrição de framework Java (e.g. Spring, Quarkus) mas será melhor avaliado se justificado no [README.md](./README.md) os motivos da decisão.

## O que iremos avaliar

Levaremos em conta os seguintes critérios:

- Cumprimento dos requisitos
- Qualidade do projeto de API e fluidez da DX
- Qualidade do layout e fluidez da UX
- Organização do código e boas práticas
- Domínio das linguagens, bibliotecas e ferramentas utilizadas
- Organização dos commits
- Escrita e cobertura de testes
