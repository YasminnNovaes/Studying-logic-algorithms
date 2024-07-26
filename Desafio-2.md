# Desafio 2.

Para dominar a programação, a prática é fundamental. Aqui você encontrará exercícios que foram propostos para que eu pudesse me exercitar e reforçar meus aprendizados em JavaScript.

---
1. Pergunte ao usuário qual é o dia da semana. Se a resposta for "Sábado" ou "Domingo", mostre "Bom fim de semana!". Caso contrário, mostre "Boa semana!".

```js
diaDaSemana = prompt('olá! que prazer te ver, que dia da semana é hoje?');
if (diaDaSemana == 'Sabado') {
  alert('Bom fim de semana!')
} else if (diaDaSemana == 'Domingo'){
  alert('Bom fim de semana!');
} else {
  alert('Boa semana!');
}
```

3. Verifique se um número digitado pelo usuário é positivo ou negativo. Mostre um alerta informando.

```js
numero = prompt('Digite um positivo ou negativo');
if (numero > 0) {
  alert('Número positivo!);
} else {
  alert('Número negativo!');
}
```

5. Crie um sistema de pontuação para um jogo. Se a pontuação for maior ou igual a 100, mostre "Parabéns, você venceu!". Caso contrário, mostre "Tente novamente para ganhar.".

```js
pontuação = 105
if (pontuação >= 100) {
  console.log('Parabéns, você venceu!');
} else {
  console.log('Tente novamente para ganhar');
}
```

7. Crie uma mensagem que informa o usuário sobre o saldo da conta, usando uma template string para incluir o valor do saldo.

```js
let saldoConta = 500
alert(`Seu saldo é de R$${saldoConta}.`);
```

8. Peça ao usuário para inserir seu nome usando prompt. Em seguida, mostre um alerta de boas-vindas usando esse nome.

```js
let nome = promt('Qual é o seu nome?');
alert(`Boas vindas ${nome`);
```
