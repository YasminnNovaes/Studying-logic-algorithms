Dados os números 12 e 13, encontre todos os divisores de cada um desses números. Sempre
considere serem números inteiros e positivos, a menos que explicitamente indicado o contrário
no enunciado. Sempre considere que os extremos (inclusive) são parte da solução a menos que
explicitamente (exclusive) estiver indicado que não se devem considerar os extremos.

#### Algoritmo

```
//Pseudocódigo

var
Numero, i, resto= inteiro

inicio
  para numero de 12 até 13 faça
    escreva("Divisores de "; numero, ": ")
      para i de 1 até numero faça
        resto := numero % i
        se resto = 0 então
          escreva(i, " ")
        fim se
      fim para
      escreva("")
  fim para
fim
```

#### Resultado esperado:

```
Divisores de 12: 1 2 3 4 6 12
Divisores de 13: 1 13
```

  
    
