# Ordenação de Três Números

Neste repositório, apresento um exercício de algoritmo que consiste em ordenar três números distintos em ordem crescente. O objetivo é demonstrar a implementação de condições para realizar a ordenação correta.

## Exercício

Dado três números positivos e distintos, imprima-os em ordem crescente.

## Algoritmo

```plaintext
Algoritmo "Ordenar_Numeros"

var
  a, b, c: inteiro

inicio
  escreva("Entre com três números positivos e distintos: ")
  leia(a)
  leia(b)
  leia(c)

  se (a <= b) e (b <= c) então
    escreva(a, ", ", b, ", ", c)
  senao
    se (a <= c) e (c <= b) então
      escreva(a, ", ", c, ", ", b)
    senao
      se (b <= a) e (a <= c) então
        escreva(b, ", ", a, ", ", c)
      senao
        se (b <= c) e (c <= a) então
          escreva(b, ", ", c, ", ", a)
        senao
          se (c <= a) e (a <= b) então
            escreva(c, ", ", a, ", ", b)
          senao
            se (c <= b) e (b <= a) então
              escreva(c, ", ", b, ", ", a)
            fimse
          fimse
        fimse
      fimse
    fimse
  fimse
fimalgoritmo
```

## Explicação do Algoritmo

1. **Declaração das Variáveis**:
   - **`a`**, **`b`**, **`c`**: Variáveis inteiras para armazenar os três números fornecidos pelo usuário.

2. **Entrada dos Números**:
   - O algoritmo solicita ao usuário que insira três números distintos e positivos.
   - Os números são lidos e armazenados nas variáveis **`a`**, **`b`** e **`c`**.

3. **Condições para Ordenar os Números**:
   - O algoritmo verifica todas as possíveis combinações de ordem para os três números e imprime-os em ordem crescente:
     - **`a <= b` e `b <= c`**: `a, b, c`
     - **`a <= c` e `c <= b`**: `a, c, b`
     - **`b <= a` e `a <= c`**: `b, a, c`
     - **`b <= c` e `c <= a`**: `b, c, a`
     - **`c <= a` e `a <= b`**: `c, a, b`
     - **`c <= b` e `b <= a`**: `c, b, a`

4. **Conclusão**:
   - O algoritmo imprime os três números em ordem crescente conforme a condição satisfeita.

<p align="center">
  <img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExenp1cmEzbnNoNWI3ZmU2bnloZndldWJuYmJubzN2MG53bGQ4bHJ1MCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT1Ra5h24Eliux3UVq/giphy.webp" alt="Ordenar números">
</p>

---

Crie seus próprios algoritmos e compartilhe seu conhecimento!
