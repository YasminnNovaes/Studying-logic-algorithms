

# Maior Número entre Dois Dados

Este repositório contém um exercício simples de algoritmos que envolve a comparação de dois números distintos para determinar o maior entre eles. O objetivo é apresentar uma solução clara e eficaz para este problema.

## Exercício

a) Dados dois números, por hipótese distintos entre si, imprima o maior deles.

b) Dados dois números, imprima o maior deles, se houver.

## Algoritmo

```plaintext
var
  n1, n2: inteiro

inicio
  escreva("Digite o primeiro número: ")
  leia(n1)
  escreva("Digite o segundo número: ")
  leia(n2)

  se n1 = n2 então
    escreva("Os números são iguais, não há número maior.")
  senão
    se n1 > n2 então
      escreva("O maior número é: ", n1)
    senão
      escreva("O maior número é: ", n2)
    fim se
  fim se
fim
```

## Explicação do Algoritmo

1. **Declaração das Variáveis**:
   - **`n1`** e **`n2`**: Variáveis inteiras que armazenam os números fornecidos pelo usuário.

2. **Entrada dos Números**:
   - O algoritmo solicita ao usuário que insira dois números. 
   - Esses números são lidos e armazenados nas variáveis **`n1`** e **`n2`**.

3. **Verificação de Igualdade**:
   - O algoritmo verifica se os dois números são iguais:
     ```plaintext
     se n1 = n2 então
       escreva("Os números são iguais, não há número maior.")
     ```
   - Se os números forem iguais, o algoritmo imprime uma mensagem informando que não há número maior.

4. **Determinação do Maior Número**:
   - Caso os números não sejam iguais, o algoritmo verifica qual é o maior:
     ```plaintext
     senão
       se n1 > n2 então
         escreva("O maior número é: ", n1)
       senão
         escreva("O maior número é: ", n2)
       fim se
     ```
   - Se **`n1`** for maior que **`n2`**, o algoritmo imprime **`n1`** como o maior número.
   - Caso contrário, imprime **`n2`** como o maior número.

5. **Conclusão**:
   - O algoritmo termina sua execução após imprimir o maior número ou informar que os números são iguais.

## Objetivo

Este exercício demonstra a capacidade de implementar condicionais para comparar números e imprimir resultados apropriados com base nas condições verificadas. É uma prática fundamental em lógica de programação e algoritmos.

---

