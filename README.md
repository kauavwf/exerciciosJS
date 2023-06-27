1.Elabore um algoritmo que leia um número, e se ele for maior do que 20, imprimir a metade desse número.

let numero = parseFloat(prompt("Digite um número:"));

if (numero > 20) {
    let metade = numero / 2;
    alert ("A metade do número é: " + metade);
}

2. Elabore um algoritmo para testar se uma senha digita é igual a “Patinho Feio”. Se a senha estiver correta escreva “Acesso permitido”, do contrario emita a mensagem “Você não tem acesso ao sistema”.
   
let senha = prompt("Digite a senha:");

if (senha === "Patinho Feio") {
    alert("Acesso permitido");
} else {
    alert("Você não tem acesso ao sistema");
}

3. Elabore um algoritmo que leia dois números inteiros e efetue a adição; caso o resultado seja maior que 10, imprima-o.
let numero1 = parseInt(prompt("Digite o primeiro número:"));
let numero2 = parseInt(prompt("Digite o segundo número:"));

let resultado = numero1 + numero2;

if (resultado > 10) {
    alert("O resultado da adição é:" + resultado);
}

4. Elabore um algoritmo que indique se um número digitado está compreendido entre 20 e 90, ou não.
   
let numero = parseInt(prompt("Digite um número:"));

if (numero >= 20 && numero <= 90) {
    alert   ("O número está compreendido entre 20 e 90.");
} else {
    alert   ("O número não está compreendido entre 20 e 90.");
}

5. Elabore um algoritmo que leia dois números e imprima o maior número.
   
let numero1 = parseFloat(prompt("Digite o primeiro número:"));
let numero2 = parseFloat(prompt("Digite o segundo número:"));

if (numero1 > numero2) {
    alert("O maior número é:"+ numero1);
} else if (numero2 > numero1) {
    alert("O maior número é:"+ numero2);
} else {
    alert("Os números são iguais.");
}

6. Elabore um algoritmo que leia dois números e imprima qual é maior e qual é menor.
   
let numero1 = parseFloat(prompt("Digite o primeiro número:"));
let numero2 = parseFloat(prompt("Digite o segundo número:"));

if (numero1 > numero2) {
    alert(numero1 + " é maior que " + numero2);
    alert(numero2 + " é menor que " + numero1);
} else if (numero2 > numero1) {
    alert(numero2 + " é maior que " + numero1);
    alert(numero1 + " é menor que " + numero2);
} else {
    alert("Os números são iguais.");
}

7. Elabore um algoritmo que leia três números e imprima o menor número.
   
let numero1 = parseFloat(prompt("Digite o primeiro número:"));
let numero2 = parseFloat(prompt("Digite o segundo número:"));
let numero3 = parseFloat(prompt("Digite o terceiro número:"));

let menor = Math.min(numero1, numero2, numero3);

alert("O menor número é:"+ menor);

8. Elabore um algoritmo que leia três números e imprima-os em ordem crescente.
let numero1 = parseFloat(prompt("Digite o primeiro número:"));
let numero2 = parseFloat(prompt("Digite o segundo número:"));
let numero3 = parseFloat(prompt("Digite o terceiro número:"));

let numeros = [numero1, numero2, numero3];
numeros.sort(function(a, b) {
    return a - b;
});

alert("Os números em ordem crescente são:"+ numeros);

9. Elabore um algoritmo que leia três números, obrigatoriamente em ordem crescente, e um quarto número que não siga esta regra.
   
let numero1 = parseFloat(prompt("Digite o primeiro número (em ordem crescente):"));
let numero2 = parseFloat(prompt("Digite o segundo número (em ordem crescente):"));
let numero3 = parseFloat(prompt("Digite o terceiro número (em ordem crescente):"));
let numero4 = parseFloat(prompt("Digite o quarto número:"));

if (numero4 < numero1) {
    alert("O quarto número não segue a ordem crescente.");
} else if (numero4 < numero2) {
    alert("O quarto número está entre o primeiro e o segundo número.");
} else if (numero4 < numero3) {
    alert("O quarto número está entre o segundo e o terceiro número.");
} else {
    alert("O quarto número é maior que o terceiro número.");
}

10. Elabore um algoritmo que leia o nome e o peso de duas pessoas e imprima o nome da pessoa mais gorda.

var nome;
var nome1;
var nome2;
var peso1;
var peso2;
var maior;

nome1=prompt("digite o seu nome");
nome2=prompt("digite outro nome");
peso1=prompt("digite seu peso");
peso2=prompt("digite outro peso");
peso1=parseFloat(peso1);
peso2=parseFloat(peso2);
if(peso1>peso2){
    maior=peso1;
    nome=nome1
    alert(  nome + " é mais pesado que " + nome2 );
}else{
    maior=peso2;
    nome=nome2;
    alert(  nome + " é mais pesado que " + nome1 );

}

11. Elabore um algoritmo que leia um número e imprima se ele é par ou ímpar. Obs: Para o número ser par, o resto de sua divisão por dois deve ser zero.

let numero = parseInt(prompt("Digite um número:"));

if (numero % 2 === 0) {
  alert("O número é par.");
} else {
  alert("O número é ímpar.");
}

12. Elabore um algoritmo que leia um número e imprima uma das mensagens: é múltiplo de 3, ou, não é múltiplo de 3.

let numero = parseInt(prompt("Digite um número:"));

if (numero % 3 === 0) {
  alert("O número é múltiplo de 3.");
} else {
  alert("O número não é múltiplo de 3.");
}

13. Faça um programa que peça uma nota, entre zero e dez. Mostre uma mensagem caso o valor seja inválido e continue pedindo até que o usuário informe um valor válido.

let nota = parseFloat(prompt("Digite uma nota entre zero e dez:"));

while (nota < 0 || nota > 10 || isNaN(nota)) {
  alert("Valor inválido. Por favor, digite uma nota entre zero e dez.");
  nota = parseFloat(prompt("Digite uma nota entre zero e dez:"));
}

alert("Valor válido informado:", nota);

14. Faça um programa que leia um nome de usuário e a sua senha e não aceite a senha igual ao nome do usuário, mostrando uma mensagem de erro e voltando a pedir as informações.

let nomeUsuario = prompt("Digite o nome de usuário:");
let senha = prompt("Digite a senha:");

while (senha === nomeUsuario) {
  alert("Erro: A senha não pode ser igual ao nome de usuário.");
  senha = prompt("Digite a senha novamente:");
}

alert("Nome de usuário:"+ nomeUsuario);
alert("Senha:"+ senha);

15. Faça um programa que leia e valide as seguintes informações:
Nome: maior que 3 caracteres;Idade: entre 0 e 150;
Salário: maior que zero; 
Sexo: 'f' ou 'm';
Estado Civil: 's', 'c', 'v', 'd';
Dica: se sua variável é texto, o tamanho dela está armazenado em: Nome.length

let nome = prompt("Digite seu nome:");
let idade = parseInt(prompt("Digite sua idade:"));
let salario = parseFloat(prompt("Digite seu salário:"));
let sexo = prompt("Digite seu sexo (f/m):");
let estadoCivil = prompt("Digite seu estado civil (s/c/v/d):");

while (nome.length <= 3 || idade < 0 || idade > 150 || salario <= 0 || (sexo !== 'f' && sexo !== 'm') || (estadoCivil !== 's' && estadoCivil !== 'c' && estadoCivil !== 'v' && estadoCivil !== 'd')) {
  alert("Alguma informação está inválida. Verifique os critérios e digite novamente.");

  nome = prompt("Digite seu nome:");
  idade = parseInt(prompt("Digite sua idade:"));
  salario = parseFloat(prompt("Digite seu salário:"));
  sexo = prompt("Digite seu sexo (f/m):");
  estadoCivil = prompt("Digite seu estado civil (s/c/v/d):");
}

alert("Informações válidas:");
alert("Nome:"+ nome);
alert("Idade:"+ idade);
alert("Salário:"+ salario);
alert("Sexo:"+ sexo);
alert("Estado Civil:"+ estadoCivil);

16. Faça um programa que imprima na tela os números de 1 a 20, um abaixo do outro. Depois modifique o programa para que ele mostre os números um ao lado do outro.

alert("Números um abaixo do outro:");
for (let i = 1; i <= 20; i++) {
  alert(i);
}

// Imprime os números um ao lado do outro
alert("Números um ao lado do outro:");
let numeros = "";
for (let i = 1; i <= 20; i++) {
  numeros += i + " ";
}
alert(numeros);

17. Faça um programa que imprima na tela apenas os números ímpares entre 1 e 50.

alert("Números ímpares entre 1 e 50:");
for (let i = 1; i <= 50; i++) {
  if (i % 2 !== 0) {
    alert(i);
  }
}

18. Faça um programa que receba dois números inteiros e gere os números inteiros que estão no intervalo compreendido por eles.

let numero1 = parseInt(prompt("Digite o primeiro número inteiro:"));
let numero2 = parseInt(prompt("Digite o segundo número inteiro:"));

alert(`Números inteiros entre ${numero1} e ${numero2}:`);
if (numero1 <= numero2) {
  for (let i = numero1; i <= numero2; i++) {
    alert(i);
  }
} else {
  for (let i = numero1; i >= numero2; i--) {
    alert(i);
  }
}
