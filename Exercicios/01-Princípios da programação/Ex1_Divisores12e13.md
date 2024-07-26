# Exercício
Dados os números 12 e 13, encontre todos os divisores de cada um desses números. Sempre
considere serem números inteiros e positivos, a menos que explicitamente indicado o contrário
no enunciado. Sempre considere que os extremos (inclusive) são parte da solução a menos que
explicitamente (exclusive) estiver indicado que não se devem considerar os extremos.

<p style="center">
  <img src="https://media.giphy.com/media/lKgyD4nD3nQXWGwiQu/giphy.gif" alt="Teacher Math Gif">
</p>


# Algoritmo

O objetivo deste algoritmo é encontrar e imprimir todos os divisores dos números 12 e 13. Ele considera que todos os números são inteiros e positivos, e inclui os extremos (1 e o próprio número) como divisores.

### Passos do Algoritmo

1. **Declaração de Variáveis:**
   - `numero`, `i`, `resto`: São declaradas como variáveis inteiras.

2. **Laço para os Números:**
   - Um laço `para` é usado para iterar de 12 até 13 (`para numero de 12 até 13 faça`).
   - Esse laço garante que o algoritmo irá encontrar divisores para ambos os números (12 e 13).

3. **Impressão dos Divisores:**
   - Para cada número (12 e 13), o algoritmo imprime uma linha indicando o número atual (`escreva("Divisores de "; numero, ": ")`).

4. **Laço para Encontrar Divisores:**
   - Um segundo laço `para` é usado para iterar de 1 até o valor do número atual (`para i de 1 até numero faça`).
   - Para cada valor de `i`, calcula o resto da divisão de `numero` por `i` (`resto := numero % i`).
   - Se o resto for 0, `i` é um divisor de `numero`, e o valor de `i` é impresso (`se resto = 0 então escreva(i, " ")`).

5. **Nova Linha Após Cada Conjunto de Divisores:**
   - Após encontrar todos os divisores de um número, uma nova linha é impressa (`escreva("")`) para separar os resultados dos dois números.

### Pseudocódigo

```plaintext
var
  Numero, i, resto: inteiro

inicio
  para numero de 12 até 13 faça
    escreva("Divisores de "; numero, ": ")
      para i de 1 até numero faça
        resto := numero % i
        se resto = 0 então
          escreva(i, " ")
        fim se
      fim para
      escreva("")
  fim para
fim
```

### Passo a Passo do Algoritmo para os Números 12 e 13

1. **Para o Número 12:**
   - Inicia `numero` em 12.
   - Imprime "Divisores de 12: ".
   - Itera `i` de 1 até 12.
     - Calcula o resto da divisão de 12 por `i`.
     - Se o resto for 0, `i` é impresso.
   - Resultado: 1 2 3 4 6 12.

2. **Para o Número 13:**
   - Incrementa `numero` para 13.
   - Imprime "Divisores de 13: ".
   - Itera `i` de 1 até 13.
     - Calcula o resto da divisão de 13 por `i`.
     - Se o resto for 0, `i` é impresso.
   - Resultado: 1 13.

### Resultado Esperado

```
Divisores de 12: 1 2 3 4 6 12
Divisores de 13: 1 13
```

  
    
