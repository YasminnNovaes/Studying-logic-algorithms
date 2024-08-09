# Algoritmo: Soma dos Números Exceto o Menor

<p align="center">
<img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExenp1cmEzbnNoNWI3ZmU2bnloZndldWJuYmJubzN2MG53bGQ4bHJ1MCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT1Ra5h24Eliux3UVq/giphy.webp" alt="Calculating GIF">
</p>

## Descrição do Exercício

O objetivo deste exercício é criar um algoritmo que solicite ao usuário "n" números inteiros e calcule a soma de todos eles, exceto o menor. É importante garantir que os números digitados sejam diferentes entre si.

## Proposta do Desafio

A proposta inicial foi realizar este exercício utilizando a estrutura de repetição tradicional `enquanto`, mas agora foi sugerido usar a estrutura `faça enquanto` para variar a abordagem e reforçar o entendimento dessa técnica.

## Algoritmo Melhorado

```pseudocode
var 
  n, i, numero, soma, menor: inteiro

Inicio 
  i := 1
  soma := 0
  menor := MAXINT
  escreva("Informe a quantidade de números a serem digitados: ")
  leia(n)

  faca
    escreva("Informe o ", i, "º número: ")
    leia(numero)

    soma := soma + numero

    se numero < menor então
      menor := numero
    fimse

    i := i + 1
  enquanto i <= n

  soma := soma - menor
  escreval("A soma dos números exceto o menor é: ", soma)
fimalgoritmo
```

## Explicação do Algoritmo

1. **Entrada dos Dados**: Primeiro, o algoritmo solicita ao usuário a quantidade de números que serão digitados.
2. **Estrutura de Repetição**: Em seguida, ele usa uma estrutura `faça enquanto` para ler cada número e acumular sua soma.
3. **Identificação do Menor Número**: Durante a repetição, o algoritmo verifica se o número atual é menor que o menor encontrado até então.
4. **Cálculo da Soma**: Após a leitura de todos os números, o algoritmo subtrai o menor número da soma total, exibindo o resultado final.
