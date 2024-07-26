# Exercicio:
Dados 3 números, apresente a soma e a média destes números.



# Algoritmo:

### Explicação do Algoritmo

O algoritmo tem o objetivo de calcular a soma e a média de três números fornecidos pelo usuário. Aqui está uma descrição passo a passo de como o algoritmo funciona:

#### 1. **Declaração das Variáveis**

```plaintext
var
  numero_1, numero_2, numero_3, soma, media: real;
```

- **`numero_1`, `numero_2`, `numero_3`**: Variáveis para armazenar os três números fornecidos pelo usuário.
- **`soma`**: Variável para armazenar o resultado da soma dos três números.
- **`media`**: Variável para armazenar o resultado da média dos três números.

#### 2. **Entrada dos Números**

```plaintext
escreva("Digite o primeiro numero: ")
leia(numero_1)

escreva("Digite o segundo numero: ")
leia(numero_2)

escreva("Digite o terceiro numero: ")
leia(numero_3)
```

- Solicita ao usuário que insira três números. Cada número é lido e armazenado nas variáveis `numero_1`, `numero_2` e `numero_3`, respectivamente.

#### 3. **Cálculo da Soma**

```plaintext
soma := numero_1 + numero_2 + numero_3
escreval("Soma dos tres numero : ", soma)
```

- Calcula a soma dos três números e armazena o resultado na variável `soma`.
- Imprime o valor da soma na tela com a mensagem "Soma dos tres numero : ".

#### 4. **Cálculo da Média**

```plaintext
media := (numero_1 + numero_2 + numero_3) / 3
escreva("Media dos tres numero : ", media)
```

- Calcula a média dos três números dividindo a soma por 3 e armazena o resultado na variável `media`.
- Imprime o valor da média na tela com a mensagem "Media dos tres numero : ".

#### 5. **Encerramento**

```plaintext
Fim
```

- Finaliza a execução do algoritmo.

### Exemplo Prático

Vamos considerar que o usuário insira os seguintes números: 4.5, 7.2 e 5.3.

1. **Entrada**:
   - `numero_1` = 4.5
   - `numero_2` = 7.2
   - `numero_3` = 5.3

2. **Cálculo da Soma**:
   - `soma = 4.5 + 7.2 + 5.3 = 17.0`
   - O algoritmo imprime: "Soma dos tres numero : 17.0"

3. **Cálculo da Média**:
   - `media = (4.5 + 7.2 + 5.3) / 3 = 17.0 / 3 ≈ 5.67`
   - O algoritmo imprime: "Media dos tres numero : 5.67"

### Algoritmo Completo em Pseudocódigo

```plaintext
Algoritmo "Soma_e_Media"

var
  numero_1, numero_2, numero_3, soma, media: real;

Inicio

  escreva("Digite o primeiro numero: ")
  leia(numero_1)

  escreva("Digite o segundo numero: ")
  leia(numero_2)

  escreva("Digite o terceiro numero: ")
  leia(numero_3)

  soma := numero_1 + numero_2 + numero_3
  escreval("Soma dos tres numero : ", soma)

  media := (numero_1 + numero_2 + numero_3) / 3
  escreva("Media dos tres numero : ", media)

Fim
```
