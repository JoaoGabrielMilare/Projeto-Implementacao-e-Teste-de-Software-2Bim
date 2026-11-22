# Estoque com TDD

Cada produto guarda seu nome e a quantidade disponível. O estoque começa em zero, acumula entradas e permite retiradas até o limite disponível.

## Decisões de implementação

Entradas e retiradas com quantidade menor ou igual a zero são ignoradas. Retirar mais do que existe também mantém a quantidade anterior.

## Testes

Os seis testes fornecidos foram preservados. Os testes adicionais verificam o nome, operações inválidas com estoque já preenchido e a retirada de todas as unidades.

## Como executar

Com JDK 17 ou superior e Maven instalados, execute nesta pasta:

    mvn test