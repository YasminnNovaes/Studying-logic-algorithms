# Soma dos Números Pares Usando "Enquanto Faça"

<p align="center">
<img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExenp1cmEzbnNoNWI3ZmU2bnloZndldWJuYmJubzN2MG53bGQ4bHJ1MCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT1Ra5h24Eliux3UVq/giphy.webp" alt="Thinking about algorithms">
</p>

## Exercício

Elabore um algoritmo que solicite ao usuário dois números inteiros e imprima a soma dos números pares existentes em seu intervalo (por exemplo, ao digitar 5 e 10, deve ser exibido 14).

## Algoritmo

```pseudocódigo
var 
  i, numero_1, numero_2, soma : inteiro;

inicio

  escreva("Informe um número inteiro: ")
  leia(numero_1)
  i := numero_1
  soma := 0

  escreva("Informe um número maior que o número anterior: ")
  leia(numero_2)

  escreval("Calculando a soma dos números pares entre ", numero_1, " e ", numero_2)

  ENQUANTO i <= numero_2 FAÇA
    se i MOD 2 = 0 ENTÃO
      soma := soma + i
    fimse
    i := i + 1
  FIMENQUANTO

  escreval("A soma dos números pares é: ", soma)

fimalgoritmo
```

## Explicação

Neste exercício, foi proposta a implementação de um algoritmo para calcular a soma dos números pares em um intervalo utilizando a estrutura de repetição "Enquanto Faça". A lógica do algoritmo envolve:

1. Solicitar ao usuário dois números inteiros que definem o intervalo.
2. Utilizar um laço "Enquanto Faça" para iterar por todos os números dentro desse intervalo.
3. Verificar se cada número é par utilizando o operador de módulo (`MOD`).
4. Somar os números pares e, ao final, exibir o resultado.

Essa abordagem permite explorar uma estrutura de repetição comum em programação e oferece um método alternativo para resolver problemas semelhantes ao uso de outros laços, como "Para".
