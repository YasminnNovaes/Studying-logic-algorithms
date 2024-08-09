Algortimo

var 
  i, numero_1, numero_2 : inteiro;

inicio

  escreva("Informe um número inteiro: ")
  leia(numero_1)
  i := numero_1

  escreva("Informe um número maior que o número anterior: ")
  leia(numero_2)

  escreval ("Listando os números pares entre ", numero_1, " e ", numero_2)

  ENQUANTO i <= 0 ENTÃO
    se i MOD 2 = 0 ENTÃO
      escreval (i)
    fimse
  fimenquanto

fimalgoritmo
