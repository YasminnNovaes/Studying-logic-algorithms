# Algoritmo para Encontrar o Maior Número

Este repositório contém um algoritmo que solicita ao usuário uma quantidade de números e encontra o maior número entre eles. O objetivo é demonstrar a capacidade de implementar loops e condicionais para resolver problemas básicos de lógica de programação.

<p align="center">
  <img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExenp1cmEzbnNoNWI3ZmU2bnloZndldWJuYmJubzN2MG53bGQ4bHJ1MCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT1Ra5h24Eliux3UVq/giphy.webp" alt="Figure It Out de Hey Arnold">
</p>

## Exercício

O exercício consiste em dois passos:

1. Solicitar a quantidade de números que o usuário deseja verificar.
2. Solicitar ao usuário que insira os números, um por um, e determinar qual deles é o maior.

## Algoritmo

```plaintext
Algoritmo "MaiorNúmero"

// Declaração das variáveis
Var
    quantidadeNumeros, i, numero, maior: Inteiro

// Início do algoritmo
Início
    // Solicita a quantidade de números que deseja verificar
    Escreva("Quantos números deseja verificar? ")
    Leia(quantidadeNumeros)

    // Verifica se a quantidade de números é válida
    Se quantidadeNumeros > 0 Então
        // Solicita o primeiro número e assume que ele é o maior inicialmente
        Escreva("Digite o número: ")
        Leia(numero)
        maior <- numero

        // Loop para solicitar os números restantes e encontrar o maior
        Para i de 2 até quantidadeNumeros Faça
            Escreva("Digite o número: ")
            Leia(numero)

            // Verifica se o número atual é maior que o maior encontrado até agora
            Se numero > maior Então
                maior <- numero
            FimSe
        FimPara

        // Imprime o maior número encontrado
        Escreva("O maior número é: ", maior)
    Senão
        Escreva("A quantidade de números deve ser maior que zero.")
    FimSe
Fim
FimAlgoritmo
```

## Explicação do Algoritmo

1. **Declaração das Variáveis**:
    - `quantidadeNumeros`, `i`, `numero`, `maior`: Variáveis inteiras utilizadas para armazenar a quantidade de números, o contador do loop, os números inseridos e o maior número encontrado, respectivamente.

2. **Entrada da Quantidade de Números**:
    - O algoritmo solicita ao usuário que insira a quantidade de números que deseja verificar. Esta quantidade é armazenada na variável `quantidadeNumeros`.

3. **Verificação da Quantidade de Números**:
    - O algoritmo verifica se a quantidade de números inserida é maior que zero. Se não for, imprime uma mensagem de erro.

4. **Entrada e Verificação dos Números**:
    - Se a quantidade de números for válida, o algoritmo solicita ao usuário que insira os números um por um. O primeiro número é assumido como o maior inicialmente.
    - O loop `Para` solicita os números restantes e, a cada iteração, verifica se o número atual é maior que o número armazenado na variável `maior`. Se for, atualiza a variável `maior`.

5. **Saída do Resultado**:
    - Após o loop, o algoritmo imprime o maior número encontrado.

## Objetivo

O objetivo deste exercício é demonstrar a habilidade de implementar estruturas de controle de fluxo (loops e condicionais) em algoritmos, bem como manipular variáveis para resolver problemas de lógica básica.
