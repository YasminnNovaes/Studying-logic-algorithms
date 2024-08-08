# Soma dos Números Pares em um intervalo

<p align="center"><img src="https://media3.giphy.com/media/3o7aTskHEUdgCQAXde/giphy.gif" alt="Coding Gif"></p>

## Exercício

Elabore um algoritmo que solicite ao usuário dois números inteiros e imprima a soma dos números pares existentes em seu intervalo (por exemplo, ao digitar 5 e 10, deve ser exibido 14).

## Algoritmo

``` 
Var
  num1, num2, soma, inicio, fim = Inteiro

Inicio
  Escreva("Digite o primeiro número: ")
  leia(num1)
  Escreva("Digite o segundo numero.")
  leia(num2)

  se(num1 = num2) então
    escreva("Os números devem ser diferentes")
  fimSe

  se(num1 < num2) então
    inicio <- num1
    fim <- num2

  senão
    inicio <- num2
    fim <- num1

  se(inicio % 2 <> 0) então
    inicio <- inicio + 1
  fimSe

  Para i de inicio até fim passo 2 faça
    soma <- soma + i
  fimPara

  escreva("A soma dos números pares entre ", num1, " e ", num2, " é: ", soma)
fim
```

## Explicação do Algoritmo

1. **Declaração e Inicialização das Variáveis**:
   - As variáveis `num1`, `num2`, `inicio`, `fim` e `soma` são declaradas como inteiros. `soma` é inicializada com 0 para acumular a soma dos números pares.

2. **Entrada dos Números**:
   - O algoritmo solicita ao usuário que insira dois números inteiros.

3. **Verificação de Números Iguais**:
   - Se os números inseridos forem iguais, o algoritmo exibe uma mensagem informando que os números devem ser diferentes e termina a execução.

4. **Definição do Intervalo**:
   - O algoritmo determina qual dos dois números inseridos é o menor (`inicio`) e qual é o maior (`fim`), definindo assim o intervalo de soma.

5. **Ajuste do Início para Par**:
   - Se `inicio` não for par, é incrementado em 1 para garantir que o laço comece a somar a partir do próximo número par.

6. **Laço para Somar Números Pares**:
   - Um laço `Para` itera de `inicio` até `fim` com passo 2, somando apenas os números pares no intervalo.

7. **Impressão do Resultado**:
   - O algoritmo imprime a soma dos números pares no intervalo especificado.

Este algoritmo garante que todos os números pares entre os dois números inseridos pelo usuário sejam somados corretamente e apresenta o resultado de forma clara e informativa.



