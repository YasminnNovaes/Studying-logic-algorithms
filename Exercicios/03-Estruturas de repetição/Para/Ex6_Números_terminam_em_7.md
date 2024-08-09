# Números que Terminam em 7

<p align="center">
<img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExdjR0d2pvcjIzNG5pOTNxaWhsM3M0NmRkNnRsN3BsNGJwaDMzNm5nNiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT9IgFgtB7U5MmugBq/giphy.webp" alt="Algorithm Thinking">
</p>

## Descrição do Exercício

Elabore um algoritmo que solicite ao usuário dois números inteiros e imprima apenas aqueles em seu intervalo que terminarem em “7” (por exemplo, ao digitar 1 e 50, deverão ser exibidos os números 7, 17, 27, 37 e 47).

## Algoritmo

```
Var
  num1, num2, inicio, fim = Inteiro

Inicio
  escreva("Digite o primeiro número: ")
  leia(num1)

  escreva("Digite o segundo número: ")
  leia(num2)

  se (num1 < num2) então
    inicio <- num1
    fim <- num2
  senão
    inicio <- num2
    fim <- num1
  fimSe

  // Ajusta o início para o próximo número que termina em 7
  se (inicio % 10 <> 7) então
    inicio <- inicio + (7 - (inicio % 10))
    se (inicio < num1 ou inicio < num2) então
      inicio <- inicio + 10
    fimSe
  fimSe

  para i de inicio até fim passo 10 faça
    se (i <= fim) então
      escreva(i," ")
    fimSe
  fimPara
fim
```

## Explicação do Algoritmo

1. **Entrada dos Números**: Solicita ao usuário dois números inteiros para definir o intervalo de busca.

2. **Definição do Intervalo**: Determina qual dos números fornecidos é menor e qual é maior para definir corretamente o início e o fim do intervalo.

3. **Ajuste do Início**: Ajusta o valor de `inicio` para o próximo número que termina em 7. Se o número inicial não termina em 7, calcula a diferença até o próximo número que termina em 7 e ajusta `inicio` de acordo.

4. **Iteração com "Para"**: Usa um laço `Para` com um passo de 10, começando do número ajustado no passo anterior, para iterar pelos números que terminam em 7.

5. **Saída dos Resultados**: Imprime todos os números dentro do intervalo que terminam em 7, garantindo que a saída seja correta e eficiente.
