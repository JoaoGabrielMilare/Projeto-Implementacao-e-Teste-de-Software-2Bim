# Carrinho de compras com TDD

O carrinho armazena uma lista de produtos e calcula o total a partir dos preços. É possível adicionar e remover produtos. Quando a soma atinge R$ 500,00, o total recebe 10% de desconto.

## Decisões de implementação

Para o requisito de preço negativo, optou-se por lançar `IllegalArgumentException` no construtor de `Produto`. Preço zero é aceito.

A remoção utiliza a mesma instância adicionada e retira uma ocorrência por chamada.

## Testes

Os testes cobrem os seis requisitos de [REQUISITOS.md](REQUISITOS.md), incluindo os valores 499,99, 500,00 e 500,01. Também verificam produtos repetidos, remoção de um produto ausente e o recálculo do desconto após remover um item.

## Como executar

Com JDK 17 ou superior e Maven instalados, execute nesta pasta:

    mvn test