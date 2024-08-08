algoritmo

var
  n, i, numero, menor, soma = Inteiro;

inicio

  menor := 9999999999
  i := 1

  escreva("Informe o numero de elementos que serão digitados: ")
  leia(n)

  Enquanto i <= n FAÇA
    escreva ("Informe o ", i, "º número inteiro positivo: ")
    leia (numero)
    se numero < menor ENTÃO
      menor := numero
    fimse
    soma := soma + numero
    i := 1 + 1
  FIMenQuANTO

  soma := soma - menor
  escreval ("A soma dos numeros digitados sem considera o menor numero é ", soma)

  fim

  
