# Subtração do Maior pelo Menor Número

Este repositório contém um exercício de algoritmos que solicita ao usuário três números inteiros e imprime a subtração do maior pelo menor.
<p align="center">
<img src="https://media.giphy.com/media/l0HlIjYveohQwpa4U/giphy.gif" alt="Figura representando subtração">
</p>

## Exercício

Elabore um algoritmo que solicite ao usuário três números inteiros e imprima a subtração do maior pelo menor. Assuma como verdade que os números informados são diferentes entre si.

## Algoritmo

```plaintext
Var
  num1: inteiro
  num2: inteiro
  num3: inteiro
  menor: inteiro
  maior: inteiro
  subtracao: inteiro

Inicio
  escreva ("Digite o primeiro numero: ")
  leia (num1)
  escreva ("Digite o segundo numero: ")
  leia (num2)
  escreva ("Digite o terceiro numero: ")
  leia (num3)

  // Encontrar o menor número
  menor := num1
  SE (num2 < menor) ENTAO
    menor := num2
  FIMSE
  SE (num3 < menor) ENTAO
    menor := num3
  FIMSE

  // Encontrar o maior número
  maior := num1
  SE (num2 > maior) ENTAO
    maior := num2
  FIMSE
  SE (num3 > maior) ENTAO
    maior := num3
  FIMSE

  subtracao := maior - menor

  escreval ("O maior numero é: ", maior)
  escreval ("O menor numero é: ", menor)
  escreval ("A subtracao do maior número pelo menor é: ", subtracao)

fimalgoritmo
```

## Explicação do Algoritmo

1. **Declaração das Variáveis**:
   - **`num1`**, **`num2`**, **`num3`**: Variáveis inteiras que armazenam os números fornecidos pelo usuário.
   - **`menor`** e **`maior`**: Variáveis para armazenar o menor e o maior número, respectivamente.
   - **`subtracao`**: Variável que armazena o resultado da subtração do maior pelo menor número.

2. **Entrada dos Números**:
   - O algoritmo solicita ao usuário que insira três números inteiros.
   - Esses números são lidos e armazenados nas variáveis **`num1`**, **`num2`** e **`num3`**.

3. **Determinação do Menor Número**:
   - Inicialmente, assumimos que **`num1`** é o menor número.
   - Comparamos **`num2`** e **`num3`** com **`menor`** e atualizamos **`menor`** conforme necessário:
     ```plaintext
     menor := num1
     SE (num2 < menor) ENTAO
       menor := num2
     FIMSE
     SE (num3 < menor) ENTAO
       menor := num3
     FIMSE
     ```

4. **Determinação do Maior Número**:
   - Inicialmente, assumimos que **`num1`** é o maior número.
   - Comparamos **`num2`** e **`num3`** com **`maior`** e atualizamos **`maior`** conforme necessário:
     ```plaintext
     maior := num1
     SE (num2 > maior) ENTAO
       maior := num2
     FIMSE
     SE (num3 > maior) ENTAO
       maior := num3
     FIMSE
     ```

5. **Cálculo da Subtração**:
   - Calculamos a subtração do maior número pelo menor e armazenamos o resultado em **`subtracao`**:
     ```plaintext
     subtracao := maior - menor
     ```

6. **Exibição dos Resultados**:
   - Exibimos o maior número, o menor número e o resultado da subtração:
     ```plaintext
     escreval ("O maior numero é: ", maior)
     escreval ("O menor numero é: ", menor)
     escreval ("A subtracao do maior número pelo menor é: ", subtracao)
     ```

## Objetivo

Este exercício demonstra a capacidade de implementar lógica de comparação e subtração em algoritmos. É uma prática fundamental em lógica de programação e desenvolvimento de algoritmos.
