# Números que Terminam em 7

<p align="center">
<img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExdjR0d2pvcjIzNG5pOTNxaWhsM3M0NmRkNnRsN3BsNGJwaDMzNm5nNiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT9IgFgtB7U5MmugBq/giphy.webp" alt="Algorithm Thinking">
</p>

## Descrição do Exercício

Elabore um algoritmo que solicite ao usuário dois números inteiros e imprima apenas aqueles em seu intervalo que terminarem em “7” (por exemplo, ao digitar 1 e 50, deverão ser exibidos os números 7, 17, 27, 37 e 47).

## Algoritmo

```
Var
  num1, num2, fim, inicio = Inteiro

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

  enquanto(inicio % 10 <> 7) faça
    inicio <- inicio + 1
  fimEnquanto

  para i de inicio até fim passo 10 faça
    escreva(i," ")
  fimPara
fim

```

## Explicação do Algoritmo

1. **Entrada dos Números**: O algoritmo solicita ao usuário dois números inteiros. Esses números definem o intervalo dentro do qual procuraremos os números que terminam em 7.

2. **Definição do Intervalo**: Verificamos qual dos números fornecidos é menor e qual é maior para definir corretamente o início e o fim do intervalo.

3. **Ajuste do Início**: Utilizamos um laço `Enquanto` para ajustar o valor de `inicio` até encontrar o próximo número que termina em 7. Isso garante que começamos a busca do ponto correto.

4. **Iteração Efetiva**: Usamos um laço `Para` com um passo de 10, começando do número ajustado no passo anterior, para iterar pelos números que terminam em 7. Isso torna o algoritmo mais eficiente.

5. **Saída dos Resultados**: O algoritmo imprime todos os números dentro do intervalo que terminam em 7, garantindo que a saída seja correta e eficiente.

## Considerações Finais

Este algoritmo é um exemplo de como podemos otimizar a busca e filtragem de dados em um intervalo, focando apenas nos resultados relevantes e reduzindo o número de iterações necessárias.
