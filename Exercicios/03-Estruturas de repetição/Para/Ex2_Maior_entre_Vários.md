# Encontrar o Maior Número entre Vários

Este repositório contém um algoritmo que solicita ao usuário uma quantidade variável de números inteiros e determina qual é o maior número. O algoritmo também verifica se todos os números fornecidos são iguais.

![Gif Exemplo](https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExenp1cmEzbnNoNWI3ZmU2bnloZndldWJuYmJubzN2MG53bGQ4bHJ1MCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT1Ra5h24Eliux3UVq/giphy.webp)

## Exercício

Elabore um algoritmo que solicite ao usuário "n" números inteiros e imprima o maior deles em tela caso haja um que seja maior que outro. Note que há a possibilidade de todos os números serem iguais.

## Algoritmo

```plaintext
Var
  n, número, maior  = inteiro
  todosIguais = lógica

Início
    Escreva("Quantos números você deseja informar?")
    Leia(n)

    Se (n > 0) Então
        
        Escreva("Digite o número 1: ")
        Leia(primeiro)
        maior <- primeiro
        todosIguais <- Verdadeiro

        
        Para i de 2 até n Faça
            Escreva("Digite o número ", i, ": ")
            Leia(numero)

            
            Se (numero > maior) Então
                maior <- numero
                todosIguais <- Falso
            Senão Se (numero < maior) Então
                todosIguais <- Falso
            FimSe
        FimPara

        
        Se (todosIguais == Verdadeiro) Então
            Escreva("Todos os números são iguais.")
        Senão
            Escreva("O maior número é: ", maior)
        FimSe
    Senão
        Escreva("Por favor, insira um número maior que zero.")
    FimSe
Fim
```

## Explicação do Algoritmo

1. **Declaração das Variáveis**:
   - **`n`**: Número de entradas que o usuário deseja informar.
   - **`numero`**: Armazena o número atual fornecido pelo usuário.
   - **`maior`**: Armazena o maior número encontrado.
   - **`primeiro`**: Armazena o primeiro número inserido para comparação.
   - **`todosIguais`**: Indica se todos os números são iguais.

2. **Entrada e Inicialização**:
   - Solicita a quantidade de números e valida se `n` é maior que zero.
   - Inicializa **`maior`** com o valor do primeiro número e define **`todosIguais`** como `Verdadeiro`.

3. **Laço para Comparação**:
   - Solicita números adicionais e compara cada um com **`maior`**.
   - Atualiza **`maior`** se um número maior for encontrado.
   - Define **`todosIguais`** como `Falso` se qualquer número for diferente do maior inicial.

4. **Resultado Final**:
   - Se **`todosIguais`** permanecer `Verdadeiro`, todos os números são iguais.
   - Caso contrário, imprime o maior número encontrado.

## Objetivo

Este exercício demonstra a capacidade de implementar algoritmos para comparar múltiplos números e verificar condições de igualdade, essencial para a lógica de programação e a resolução de problemas complexos.
