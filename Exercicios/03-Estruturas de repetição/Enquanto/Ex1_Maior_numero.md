# Encontrando o Maior Número

<p align="center">
<img src="https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExMDRvcHQxbXc5d3JjZHJ4YnZqcjFqcG5keDhvdXI1ZGFvajBsdXBubyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/lVN6g7CNgshTtPiG8m/giphy.webp" alt="Gif de Análise de Números">
</p>

## Descrição do Exercício

O exercício consiste em dois passos:

1. Solicitar uma quantidade de números que o usuário deseja verificar.
2. Solicitar ao usuário que insira os números, um por um, e determinar qual deles é o maior.

Neste exemplo, o algoritmo foi ajustado para utilizar a estrutura de repetição **ENQUANTO**, realizando a verificação dos números digitados pelo usuário até que todos sejam processados.

## Algoritmo

```
Var 
  n, i, numero, maior: inteiro;

Inicio

  escreva("Informe o número de elementos que serão digitados: ")
  leia(n)

  i := 1
  maior := -1 // Inicializa com um valor que garantidamente será menor que qualquer número positivo digitado

  ENQUANTO i <= n FAÇA
    escreva ("Informe o ", i, "º número inteiro positivo: ")
    leia (numero)
    
    SE numero > maior ENTÃO
      maior := numero
    FIM SE
    
    i := i + 1
  FIM ENQUANTO

  escreva ("O maior número digitado foi ", maior)

Fimalgoritmo
```

## Explicação do Algoritmo

Este algoritmo foi criado para solicitar ao usuário um número `n` de elementos a serem inseridos, e depois encontrar e imprimir o maior número entre os valores informados. O algoritmo usa a estrutura de repetição **ENQUANTO** para iterar sobre todos os números inseridos pelo usuário.

### Proposta de Melhoria

Diferente de outras abordagens, aqui a estrutura **ENQUANTO** é utilizada para garantir que todos os elementos sejam verificados antes de finalizar a execução. Além disso, foram feitos ajustes para garantir que o algoritmo funcione corretamente em todas as situações, como a inicialização adequada da variável `maior`.
