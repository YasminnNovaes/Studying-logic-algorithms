# Números que Terminam em 7

<p align="center">
  <img src="https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExMjg5eW0zODliamxvbDdxbnpuZzRhaTdpOXk5OW1vMmh2b3IxaHA2eSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/l4Ho74sS3cxg5TLLa/giphy.webp" alt="Numbers GIF">
</p>

## Exercício

Elabore um algoritmo que solicite ao usuário dois números inteiros e imprima apenas aqueles em seu intervalo que terminarem em "7". Por exemplo, ao digitar 1 e 50, deverão ser exibidos os números 7, 17, 27, 37 e 47.

## Algoritmo

```plaintext
var
  i, numero_1, numero_2 = inteiro

inicio
  escreva("Informe um número inteiro: ")
  leia(numero_1)

  escreva("Informe um número inteiro maior que o número anterior: ")
  leia(numero_2)

  i := numero_1 + 1

  Enquanto i <= numero_2 - 1 FAÇA
    se i % 10 = 7 ENTÃO
      escreva(i, " ")
    fimse
    i := i + 1
  FIMENQUANTO
fim
```

## Explicação do Algoritmo

Este algoritmo foi desenvolvido para solicitar ao usuário dois números inteiros e imprimir apenas os números dentro desse intervalo que terminam em "7". O processo foi feito usando a estrutura de repetição "ENQUANTO FAÇA", que permite uma execução contínua do bloco de código até que a condição estabelecida não seja mais satisfeita.

### Como Funciona

1. **Entrada dos Dados**: O algoritmo começa solicitando ao usuário dois números inteiros. O primeiro número (`numero_1`) é o início do intervalo, e o segundo (`numero_2`) é o final.

2. **Inicialização**: A variável `i` é inicializada com `numero_1 + 1`, para começar a verificação logo após o primeiro número fornecido.

3. **Repetição com Condição**: Enquanto `i` for menor ou igual a `numero_2 - 1`, o algoritmo verifica se o número termina em "7". Isso é feito verificando se o resto da divisão de `i` por 10 é igual a 7 (`i % 10 = 7`).

4. **Saída dos Dados**: Se o número terminar em "7", ele é impresso. A variável `i` é então incrementada em 1, e o processo se repete até que `i` exceda `numero_2 - 1`.

### Observações

Este exercício foi proposto para ser resolvido utilizando a estrutura de repetição "ENQUANTO FAÇA", proporcionando uma maneira diferente de abordar problemas semelhantes, tornando o algoritmo mais versátil e adaptável a diferentes cenários.
