1.Elabore um algoritmo que leia um número, e se ele for maior do que 20, imprimir a metade desse número.


2. Elabore um algoritmo para testar se uma senha digita é igual a “Patinho Feio”. Se a senha estiver correta escreva “Acesso permitido”, do contrario emita a mensagem “Você não tem acesso ao sistema”.


3. Elabore um algoritmo que leia dois números inteiros e efetue a adição; caso o resultado seja maior que 10, imprima-o.


4. Elabore um algoritmo que indique se um número digitado está compreendido entre 20 e 90, ou não.


5. Elabore um algoritmo que leia dois números e imprima o maior número.


6. Elabore um algoritmo que leia dois números e imprima qual é maior e qual é menor.


7. Elabore um algoritmo que leia três números e imprima o menor número.


8. Elabore um algoritmo que leia três números e imprima-os em ordem crescente.


9. Elabore um algoritmo que leia três números, obrigatoriamente em ordem crescente, e um quarto número que não siga esta regra. 


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


12. Elabore um algoritmo que leia um número e imprima uma das mensagens: é múltiplo de 3, ou, não é múltiplo de 3.


13. Faça um programa que peça uma nota, entre zero e dez. Mostre uma mensagem caso o valor seja inválido e continue pedindo até que o usuário informe um valor válido.


14. Faça um programa que leia um nome de usuário e a sua senha e não aceite a senha igual ao nome do usuário, mostrando uma mensagem de erro e voltando a pedir as informações.


15. Faça um programa que leia e valide as seguintes informações:
Nome: maior que 3 caracteres;Idade: entre 0 e 150;
Salário: maior que zero; 
Sexo: 'f' ou 'm';
Estado Civil: 's', 'c', 'v', 'd';
Dica: se sua variável é texto, o tamanho dela está armazenado em: Nome.length


16. Faça um programa que imprima na tela os números de 1 a 20, um abaixo do outro. Depois modifique o programa para que ele mostre os números um ao lado do outro.


17. Faça um programa que imprima na tela apenas os números ímpares entre 1 e 50.


18. Faça um programa que receba dois números inteiros e gere os números inteiros que estão no intervalo compreendido por eles.