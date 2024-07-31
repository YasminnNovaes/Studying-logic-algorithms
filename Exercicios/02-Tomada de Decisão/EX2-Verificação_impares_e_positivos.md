# Verificação de Números Positivos e Ímpares

<p align="center">
  <img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExenp1cmEzbnNoNWI3ZmU2bnloZndldWJuYmJubzN2MG53bGQ4bHJ1MCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT1Ra5h24Eliux3UVq/giphy.webp" alt="Math Gif">
</p>

Este repositório contém um exercício simples de algoritmos que envolve a verificação de dois números para determinar se ambos são positivos, ímpares, ou outros casos.

## Exercício

Dados dois números, imprima "azul" se ambos forem positivos, "laranja" se ambos forem ímpares ou "roxo" nos demais casos.

## Algoritmo

```plaintext
Var
  n1, n2: inteiro
  teste1, teste2: lógico
fim variavel

Inicio
  escreva("Digite o primeiro número: ")
  leia(n1)
  escreva("Digite o segundo número: ")
  leia(n2)

  // Verifica se ambos os números são positivos
  teste1 := (n1 > 0) e (n2 > 0)
  
  // Verifica se ambos os números são ímpares
  teste2 := (n1 mod 2 = 1) e (n2 mod 2 = 1)

  se teste1 então
    escreva("azul")
  senão
    se teste2 então
      escreva("laranja")
    senão
      escreva("roxo")
    fim se
  fim se
fim
```

## Explicação do Algoritmo

1. **Declaração das Variáveis**:
   - **`n1`** e **`n2`**: Variáveis inteiras para armazenar os números fornecidos pelo usuário.
   - **`teste1`** e **`teste2`**: Variáveis lógicas para armazenar os resultados das condições.

2. **Entrada dos Números**:
   - O algoritmo solicita ao usuário que insira dois números e os armazena nas variáveis **`n1`** e **`n2`**.

3. **Verificação Lógica**:
   - **`teste1 := (n1 > 0) e (n2 > 0)`**: Verifica se ambos os números são positivos.
   - **`teste2 := (n1 mod 2 = 1) e (n2 mod 2 = 1)`**: Verifica se ambos os números são ímpares.

4. **Estrutura Condicional**:
   - **`se teste1 então`**: Se ambos os números são positivos, imprime "azul".
   - **`senão`**: Caso contrário,
     - **`se teste2 então`**: Se ambos os números são ímpares, imprime "laranja".
     - **`senão`**: Nos demais casos, imprime "roxo".

## Objetivo

Este exercício demonstra a capacidade de implementar condicionais para verificar múltiplas condições e imprimir resultados apropriados com base nas condições verificadas. É uma prática fundamental em lógica de programação e algoritmos.

---
