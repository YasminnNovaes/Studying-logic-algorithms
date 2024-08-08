Algoritmo

Var
  n, i, numero, menor, soma = Inteiro

inicio
  menor := 99999999999999
  i := 1

  escreva("Informe o número de elementos que serão digitados; ")
  leia(n)

  ENQUANTO i <= n FACA
    escreva ("Informe o ", i, "/º número inteiro positivo: ")
    leia (numero)
    se numero < menor ENTÃO
      menor := numero
    fimse
    soma := soma + numero
    i := i + 1
  FIMENQUANTO
  soma := soma - menor
  media := soma / (n-1)
  escreval
