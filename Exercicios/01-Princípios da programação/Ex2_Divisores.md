# Exercicio proposto:

Escreva um algoritmo que descreva a maneira de encontrar todos os divisores de um número
qualquer.
Comece a contagem em 1.
Divida o número desejado pelo número que está na contagem.
Se o resto da divisão for zero, considere o valor que está na contagem como um dos divisores
do número.
Incremente o valor da contagem em 1.
Repita as operações anteriores até que o número da contagem seja superior ao número que
desejamos descobrir os divisores.

### Algoritmo realizado:
```
var
  numero, i, resto: inteiro

inicio
  Escreva("Digite um numero: ")
  leia(numero)
  
  para i de 1 até numero faça
    resto := numero % i
    se resto = 0 então
      escreva(i, " ")
    fim se
  fim para
fim
```

# Explicação do Algoritmo

1. **Declaração das Variáveis:**
   - `numero`, `i` e `resto` são declarados como inteiros.

2. **Entrada do Usuário:**
   - Solicita ao usuário para digitar um número (`numero`).

3. **Laço `para`:**
   - O laço começa em 1 (`para i de 1`) e vai até o valor de `numero` (`até numero`).
   - A variável `resto` armazena o resto da divisão de `numero` por `i`.
   - Se `resto` for 0, significa que `i` é um divisor de `numero`, e então `i` é impresso.

Para garantir que o algoritmo está funcionando corretamente, vamos considerar um exemplo:

- Se `numero` for 6:
  - A saída deverá ser: `1 2 3 6`

O algoritmo corrigido deve encontrar e imprimir corretamente todos os divisores do número fornecido.
