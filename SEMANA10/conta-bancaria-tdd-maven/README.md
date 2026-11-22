# Conta bancária com TDD

A conta inicia com saldo zero. Os depósitos se acumulam e os saques são realizados quando há saldo suficiente. Uma tentativa de saque acima do saldo é ignorada, conforme o teste fornecido.

## Decisões de implementação

Também são ignorados valores negativos, zero e valores não finitos, como `NaN` e infinito.

## Testes

Os quatro testes originais foram preservados, com testes adicionais para saldo inicial, saque de todo o saldo e operações inválidas.

## Como executar

Com JDK 17 ou superior e Maven instalados, execute nesta pasta:

    mvn test
