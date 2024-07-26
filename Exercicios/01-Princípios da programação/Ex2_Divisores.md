# Exercicio:

Escreva um algoritmo que descreva a maneira de encontrar todos os divisores de um número
qualquer.
Comece a contagem em 1.
Divida o número desejado pelo número que está na contagem.
Se o resto da divisão for zero, considere o valor que está na contagem como um dos divisores
do número.
Incremente o valor da contagem em 1.
Repita as operações anteriores até que o número da contagem seja superior ao número que
desejamos descobrir os divisores.

<p align="center">
<img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExenp1cmEzbnNoNWI3ZmU2bnloZndldWJuYmJubzN2MG53bGQ4bHJ1MCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT1Ra5h24Eliux3UVq/giphy.webp" alt="Figure It Out de Hey Arnold">
</p>



# Explicação do Algoritmo

O objetivo deste algoritmo é encontrar e exibir todos os divisores de um número inteiro positivo fornecido pelo usuário. O algoritmo segue estes passos:

1. **Declaração das Variáveis:**
   - `numero`: Armazena o número para o qual queremos encontrar os divisores.
   - `i`: Variável usada como contador no laço que vai de 1 até o valor de `numero`.
   - `resto`: Armazena o resultado da operação de módulo, que indica se `i` é um divisor de `numero`.

2. **Entrada do Usuário:**
   - O algoritmo solicita ao usuário que insira um número (`Escreva("Digite um numero: ")`).
   - O valor digitado é lido e armazenado na variável `numero` (`leia(numero)`).

3. **Laço de Contagem:**
   - Um laço `para` é utilizado para iterar `i` de 1 até o valor de `numero` (`para i de 1 até numero faça`).
   - Para cada valor de `i`, o algoritmo calcula o resto da divisão de `numero` por `i` (`resto := numero % i`).
   - Se o resto da divisão for 0 (`se resto = 0 então`), significa que `i` é um divisor de `numero`, e `i` é impresso na tela (`escreva(i, " ")`).

4. **Conclusão do Laço:**
   - O laço continua até que `i` atinja o valor de `numero`.
   - Após completar o laço, o algoritmo encerra (`fim`).

### Funcionamento do Algoritmo

1. **Entrada:**
   - Suponha que o usuário insira o número 12.

2. **Execução do Laço:**
   - O laço percorre todos os valores de `i` de 1 até 12.
   - Para cada valor de `i`, o resto da divisão de 12 por `i` é calculado.
   - Se o resto for 0, `i` é um divisor de 12 e é impresso.

3. **Resultado:**
   - Para o número 12, o algoritmo encontra e imprime os divisores: 1, 2, 3, 4, 6 e 12.

### Algoritmo Completo em Pseudocódigo

```plaintext
var
  numero, i, resto: inteiro

inicio
  Escreva("Digite um numero: ")
  leia(numero)
  
  para i de 1 até numero faça
    resto := numero % i
    se resto = 0 então
      escreva(i, " ")
    fim se
  fim para
fim
```

### Explicação do Pseudocódigo

- **Declaração das Variáveis:** Define as variáveis necessárias (`numero`, `i`, `resto`).
- **Entrada do Número:** Solicita ao usuário o número a ser verificado.
- **Laço para Encontrar Divisores:** Itera sobre todos os números de 1 até `numero`, verificando se cada número é um divisor.
- **Impressão dos Divisores:** Exibe cada divisor encontrado.

### Resultado Esperado

O algoritmo deve imprimir todos os divisores do número fornecido pelo usuário, separados por espaços.
