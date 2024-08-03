# Cálculo da Média dos Números Exceto o Menor

Este repositório contém um algoritmo que solicita ao usuário uma quantidade de números inteiros e calcula a média desses números, excluindo o menor deles. Assumimos que todos os números fornecidos são distintos entre si.

<p align="center">
  <img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExenp1cmEzbnNoNWI3ZmU2bnloZndldWJuYmJubzN2MG53bGQ4bHJ1MCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT1Ra5h24Eliux3UVq/giphy.webp" alt="Computação">
</p>

## Exercício

Elabore um algoritmo que solicite ao usuário "n" números inteiros e calcule a média desses números, excluindo o menor deles. Assuma que todos os números digitados serão diferentes entre si.

## Algoritmo

```

Var
    n, numero, menor, soma = Inteiro
    media = Real

Início
    Escreva("Quantos números você deseja informar?")
    Leia(n)

    Se (n > 1) Então

        Escreva("Digite o número 1: ")
        Leia(numero)
        menor <- numero
        soma <- numero

        Para i de 2 até n Faça
            Escreva("Digite o número ", i, ": ")
            Leia(numero)

            Se (numero < menor) Então
                menor <- numero
            FimSe

            soma <- soma + numero
        FimPara

        media <- (soma - menor) / (n - 1)

        Escreva("A média dos números, exceto o menor, é: ", media)
    Senão
        Escreva("Por favor, insira um número maior que 1.")
    FimSe
Fim
```

## Explicação do Algoritmo

1. **Declaração das Variáveis**:
   - **`n`**: Número total de inteiros que o usuário deseja fornecer.
   - **`numero`**: Armazena cada número fornecido pelo usuário.
   - **`menor`**: Armazena o menor número entre os fornecidos.
   - **`soma`**: Armazena a soma total dos números fornecidos.
   - **`media`**: Armazena a média dos números, excluindo o menor.

2. **Entrada e Inicialização**:
   - Solicita o número de inteiros e valida se `n` é maior que 1.
   - Solicita o primeiro número e inicializa **`menor`** e **`soma`** com esse número.

3. **Laço para Processamento**:
   - Solicita os números adicionais e atualiza **`menor`** se o número atual for menor.
   - Atualiza **`soma`** com o número atual.

4. **Cálculo e Resultado**:
   - Calcula a média excluindo o menor número.
   - Imprime a média dos números, excluindo o menor.

## Objetivo

Este exercício demonstra como processar uma lista de números para atender a uma condição específica e é útil para entender o uso de variáveis, laços e condicionais em algoritmos.
