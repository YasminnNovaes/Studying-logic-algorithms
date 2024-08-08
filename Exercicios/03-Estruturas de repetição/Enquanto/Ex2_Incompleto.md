

Exercicio

Algoritmo

var 
  n, i, numero, maior = Inteiro
  repetido = lógico

Inicio 

  i := 1
  escreva("Informe o numero de elementos que serão digitados: ")
  leia(n)

  Enquanto i <= n FAÇA
    escreva ("Informe o ", i, "º número inteiro positivo: ")
    leia (numero)
    se numero = maior ENTÃO
      repetido := verdadeiro
    fimse
    se numero > maior  ENTÂO
      maior := numero
    fimse
    i := i+1
  FIMENQUANTO

  escreval ("O maior número digitado foi ", maior)

  se (repetido) ENTÂO
    escreva("Existem números repetidos na sequencia de números")
  fimse

fimalgoritmo
````

