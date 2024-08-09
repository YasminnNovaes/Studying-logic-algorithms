algoritmo 

var
  i, numero_1, numero_2, soma = inteiro

inicio

  escreva("Informe um número inteiro: ")
  leia(numero_1)
  i := numero_1 +1

  escreva("Informe um número inteiro maior que o número anterior: ")
  leia(numero_2)

  Enquanto i <= numero_2 -1 FAÇA
    se i MOD 2 = 0 ENTÃO
      soma := soma + 1
    fimse
    i := i + 1
  FIMENQUANTO

  escreva("A soma dos pares é : ", soma)

fim
