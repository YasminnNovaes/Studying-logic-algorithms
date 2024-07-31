# Verificação de Paridade de Números

Este repositório contém um exercício de algoritmos que verifica a paridade de dois números inteiros e positivos fornecidos pelo usuário. O objetivo é imprimir se ambos são pares, ambos são ímpares ou se há uma mistura de par e ímpar.

<p align="center">
<img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExenp1cmEzbnNoNWI3ZmU2bnloZndldWJuYmJubzN2MG53bGQ4bHJ1MCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT1Ra5h24Eliux3UVq/giphy.webp" alt="Figura representando pensamento lógico">
</p>

## Exercício

Elabore um algoritmo que solicite ao usuário dois números inteiros e positivos. Imprima “Pares” se ambos forem pares, “Ímpares” se ambos forem ímpares ou “Outro” nos demais casos.

## Algoritmo

```plaintext
var
  n1, n2: inteiro

inicio
  escreva("Digite dois números inteiros e positivos: ")
  leia(n1, n2)

  se (n1 % 2 = 0) e (n2 % 2 = 0) então
    escreval("Pares")
  senao
    se (n1 % 2 = 1) e (n2 % 2 = 1) então
      escreval("Ímpares")
    senao
      escreval("Outro")
    fim se
  fim se
fim
```

## Explicação do Algoritmo

1. **Declaração das Variáveis**:
   - **`n1`** e **`n2`**: Variáveis inteiras que armazenam os números fornecidos pelo usuário.

2. **Entrada dos Números**:
   - O algoritmo solicita ao usuário que insira dois números inteiros e positivos.
   - Esses números são lidos e armazenados nas variáveis **`n1`** e **`n2`**.

3. **Verificação das Condições**:
   - O algoritmo verifica se ambos os números são pares:
     ```plaintext
     se (n1 % 2 = 0) e (n2 % 2 = 0) então
       escreval("Pares")
     ```
   - Se ambos os números forem pares, imprime "Pares".
   
   - Se a condição acima não for satisfeita, o algoritmo verifica se ambos os números são ímpares:
     ```plaintext
     senao
       se (n1 % 2 = 1) e (n2 % 2 = 1) então
         escreval("Ímpares")
       ```
     - Se ambos os números forem ímpares, imprime "Ímpares".
   
   - Se nenhuma das condições anteriores for satisfeita, o algoritmo imprime "Outro":
     ```plaintext
       senao
         escreval("Outro")
       fim se
     fim se
     ```

4. **Conclusão**:
   - O algoritmo termina sua execução após imprimir a mensagem correspondente à condição verificada.

## Objetivo

Este exercício demonstra a capacidade de implementar condicionais para verificar a paridade de números e imprimir resultados apropriados com base nas condições verificadas. É uma prática fundamental em lógica de programação e algoritmos.
