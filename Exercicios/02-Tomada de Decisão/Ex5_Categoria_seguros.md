# Classificação de Categoria de Seguro

<p align="center">
<img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExenp1cmEzbnNoNWI3ZmU2bnloZndldWJuYmJubzN2MG53bGQ4bHJ1MCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT1Ra5h24Eliux3UVq/giphy.webp" alt="Gif Ilustrativo">
</p>

## Exercício

Certa companhia de seguros possui nove categorias de seguro, em função da idade e do tipo de trabalho do segurado, conforme a tabela abaixo:

| Idade  | Baixo Risco | Médio Risco |
|--------|--------------|-------------|
| 17 a 20 | 1            | 2           |
| 21 a 24 | 2            | 3           |
| 25 a 34 | 3            | 4           |
| 35 a 64 | 4            | 5           |
| 65 a 70 | 7            | 8           |

Elabore um algoritmo que solicite ao usuário a idade e o nível de risco ("B" para "baixo risco", "M" para "médio risco" e "A" para "alto risco") e, a partir deles, calcule a categoria do seguro, exibindo o número de 1 a 9 na tela.

## Algoritmo

```plaintext
var
  idade: inteiro;
  risco: caractere;

inicio
  escreva("Informe a idade do segurado: ")
  leia(idade)

  se (idade < 17) ou (idade > 70) então
    escreval("Idade fora dos limites permitidos.")
  senão
    escreva("Informe a categoria de risco do segurado (B, M ou A): ")
    leia(risco)

    se (idade >= 17) e (idade <= 20) então
      escolha (risco)
        caso 'B'
          escreval("Categoria de risco 1")
        caso 'M'
          escreval("Categoria de risco 2")
        caso 'A'
          escreval("Categoria de risco 3")
        outrocaso
          escreval("Categoria de risco inválida")
      fimescolha
    senão
      se (idade >= 21) e (idade <= 24) então
        escolha (risco)
          caso 'B'
            escreval("Categoria de risco 2")
          caso 'M'
            escreval("Categoria de risco 3")
          caso 'A'
            escreval("Categoria de risco 4")
          outrocaso
            escreval("Categoria de risco inválida")
        fimescolha
      senão
        se (idade >= 25) e (idade <= 34) então
          escolha (risco)
            caso 'B'
              escreval("Categoria de risco 3")
            caso 'M'
              escreval("Categoria de risco 4")
            caso 'A'
              escreval("Categoria de risco 5")
            outrocaso
              escreval("Categoria de risco inválida")
          fimescolha
        senão
          se (idade >= 35) e (idade <= 64) então
            escolha (risco)
              caso 'B'
                escreval("Categoria de risco 4")
              caso 'M'
                escreval("Categoria de risco 5")
              caso 'A'
                escreval("Categoria de risco 6")
              outrocaso
                escreval("Categoria de risco inválida")
            fimescolha
          senão
            se (idade >= 65) e (idade <= 70) então
              escolha (risco)
                caso 'B'
                  escreval("Categoria de risco 7")
                caso 'M'
                  escreval("Categoria de risco 8")
                caso 'A'
                  escreval("Categoria de risco 9")
                outrocaso
                  escreval("Categoria de risco inválida")
              fimescolha
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
   - `idade`: Variável inteira para armazenar a idade do segurado.
   - `risco`: Variável caractere para armazenar a categoria de risco (`B`, `M` ou `A`).

2. **Entrada da Idade**:
   - O algoritmo solicita ao usuário que informe a idade do segurado.
   - Se a idade estiver fora dos limites permitidos (menor que 17 ou maior que 70), o algoritmo imprime uma mensagem de erro e termina.

3. **Entrada da Categoria de Risco**:
   - Se a idade estiver dentro dos limites permitidos, o algoritmo solicita ao usuário que informe a categoria de risco do segurado.

4. **Determinação da Categoria de Risco**:
   - Para cada faixa etária (17-20, 21-24, 25-34, 35-64, 65-70), o algoritmo verifica a categoria de risco (`B`, `M`, ou `A`) e imprime a categoria correspondente.
   - Se o caractere de risco não for válido (`B`, `M`, ou `A`), o algoritmo imprime uma mensagem de erro.

5. **Fim do Algoritmo**:
   - O algoritmo termina sua execução após determinar e imprimir a categoria de risco ou uma mensagem de erro.

---
