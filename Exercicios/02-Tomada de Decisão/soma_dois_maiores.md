# Soma dos Dois Maiores Números

Este repositório contém um exercício que demonstra como encontrar e somar os dois maiores números entre três números distintos fornecidos pelo usuário. O objetivo é apresentar uma solução clara e eficaz para este problema.

<p align="center">
<img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExenp1cmEzbnNoNWI3ZmU2bnloZndldWJuYmJubzN2MG53bGQ4bHJ1MCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT1Ra5h24Eliux3UVq/giphy.webp" alt="Figure It Out de Hey Arnold">
</p>

## Exercício

Dados três números, necessariamente distintos entre si, imprima a soma dos dois maiores.

## Algoritmo

```plaintext
Var
  num1: real
  num2: real
  num3: real
  menor: real
  soma: real

Inicio
  menor := 99999999999999999999
  soma := 0

  escreva("Digite o primeiro número: ")
  leia(num1)

  escreva("Digite o segundo número: ")
  leia(num2)

  escreva("Digite o terceiro número: ")
  leia(num3)

  SE num1 < menor ENTÃO
    menor := num1
  FIMSE

  SE num2 < menor ENTÃO
    menor := num2
  FIMSE

  SE num3 < menor ENTÃO
    menor := num3
  FIMSE

  SE num1 <> menor ENTÃO
    soma := soma + num1
  FIMSE

  SE num2 <> menor ENTÃO
    soma := soma + num2
  FIMSE

  SE num3 <> menor ENTÃO
    soma := soma + num3
  FIMSE

  escreval("O menor número é: ", menor)
  escreval("A soma dos 2 maiores números é: ", soma)
fimalgoritmo
```

## Explicação do Algoritmo

1. **Declaração das Variáveis**:
   - **`num1, num2, num3`**: Variáveis reais para armazenar os números fornecidos pelo usuário.
   - **`menor`**: Variável real para armazenar o menor número entre os três.
   - **`soma`**: Variável real para armazenar a soma dos dois maiores números.

2. **Inicialização das Variáveis**:
   - **`menor`** é inicializada com um valor muito alto para garantir que qualquer número fornecido pelo usuário será menor.
   - **`soma`** é inicializada com 0.

3. **Entrada dos Números**:
   - O algoritmo solicita ao usuário que insira três números e os armazena nas variáveis **`num1, num2, num3`**.

4. **Determinação do Menor Número**:
   - O algoritmo verifica se **`num1`**, **`num2`** ou **`num3`** são menores que o valor atual de **`menor`** e atualiza **`menor`** se a condição for verdadeira.

5. **Cálculo da Soma dos Dois Maiores Números**:
   - O algoritmo adiciona **`num1`**, **`num2`** e **`num3`** a **`soma`** se eles não forem iguais ao valor de **`menor`**.

6. **Impressão dos Resultados**:
   - O algoritmo imprime o menor número e a soma dos dois maiores números.

## Objetivo

Este exercício demonstra a capacidade de implementar lógica condicional para determinar o menor número e calcular a soma dos dois maiores entre três números distintos. É uma prática fundamental em lógica de programação e algoritmos.

---

Crie uma conta no GitHub e compartilhe seu conhecimento!
