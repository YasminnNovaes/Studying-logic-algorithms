### Média com Exclusão do Menor Número

<p align="center">
<img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExenp1cmEzbnNoNWI3ZmU2bnloZndldWJuYmJubzN2MG53bGQ4bHJ1MCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/xT1Ra5h24Eliux3UVq/giphy.webp" alt="Figure It Out de Hey Arnold">
</p>

---

### Exercício

Elabore um algoritmo que solicite ao usuário "n" números inteiros e calcule a média desses números, excluindo o menor deles. Assuma que todos os números digitados serão diferentes entre si.

### Algoritmo

```pseudocode
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
  escreva("A média dos números, excluindo o menor, é: ", media)
```

### Explicação do Algoritmo

Neste algoritmo, a proposta é calcular a média de "n" números inteiros fornecidos pelo usuário, excluindo o menor número da média. Para isso, utilizamos a estrutura de repetição "ENQUANTO FAÇA", que continua solicitando os números até que todos tenham sido inseridos.

Primeiro, o algoritmo inicializa a variável `menor` com um valor extremamente alto, garantindo que qualquer número fornecido pelo usuário será menor do que esse valor inicial. Em seguida, o programa solicita a quantidade de números que serão inseridos, e em seguida, no loop "ENQUANTO", ele recebe os números, verifica se o número atual é menor que o menor valor registrado, e soma os números.

Após o loop, o menor número é subtraído da soma total e, em seguida, a média é calculada com base nos "n-1" números restantes. Por fim, a média é exibida para o usuário.
