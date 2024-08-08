# Soma dos Números Exceto o Menor

Este repositório contém um algoritmo que solicita ao usuário uma quantidade de números inteiros e calcula a soma de todos os números fornecidos, excluindo o menor deles. É assumido que todos os números fornecidos são distintos.

<p align="center">
  <img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExenp1cmEzbnNoNWI3ZmU2bnloZndldWJuYmJubzN2MG53bGQ4bHJ1MCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT1Ra5h24Eliux3UVq/giphy.webp" alt="Soma dos Números">
</p>

## Exercício

Elabore um algoritmo que solicite ao usuário "n" números inteiros e imprima a soma de todos os números, exceto o menor deles. Assumir que os números digitados serão diferentes entre si.

## Algoritmo

```plaintext
Início
    // Declaração das variáveis
    Inteiro n, numero, soma, menor

    // Solicita a quantidade de números que o usuário deseja informar
    Escreva("Quantos números você deseja informar?")
    Leia(n)

    // Verifica se n é maior que zero
    Se (n > 0) Então
        // Solicita o primeiro número e inicializa 'menor' e 'soma'
        Escreva("Digite o número 1: ")
        Leia(numero)
        menor <- numero
        soma <- numero

        // Laço para solicitar e processar os números restantes
        Para i de 2 até n Faça
            Escreva("Digite o número ", i, ": ")
            Leia(numero)

            // Atualiza menor e soma
            Se (numero < menor) Então
                menor <- numero
            FimSe

            soma <- soma + numero
        FimPara

        // Calcula a soma excluindo o menor número
        soma <- soma - menor

        // Imprime o resultado
        Escreva("A soma dos números, exceto o menor, é: ", soma)
    Senão
        Escreva("Por favor, insira um número maior que zero.")
    FimSe
Fim
```

## Explicação do Algoritmo

1. **Declaração das Variáveis**:
   - **`n`**: Número de inteiros que o usuário deseja fornecer.
   - **`numero`**: Armazena cada número fornecido pelo usuário.
   - **`soma`**: Armazena a soma total dos números fornecidos.
   - **`menor`**: Armazena o menor número entre os fornecidos.

2. **Entrada e Inicialização**:
   - Solicita o número de inteiros e valida se `n` é maior que zero.
   - Solicita o primeiro número e inicializa tanto a **`menor`** quanto a **`soma`** com esse número.

3. **Laço para Processamento**:
   - Solicita os números adicionais e atualiza **`menor`** se o número atual for menor.
   - Atualiza **`soma`** com o número atual.

4. **Cálculo e Resultado**:
   - Subtrai o menor número da soma total.
   - Imprime a soma dos números, excluindo o menor.

## Objetivo

Este exercício demonstra como processar uma lista de números para atender a uma condição específica e é útil para entender o uso de variáveis, laços e condicionais em algoritmos.
