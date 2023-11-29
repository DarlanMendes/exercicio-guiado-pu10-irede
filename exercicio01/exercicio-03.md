# Exercício 03 - Funções, escopo de variáveis e gerenciamento de módulos
01 - Crie uma função que receba 05 argumentos e retorne-os em ordem alfabética.
Restrições:
- Se receber como argumento algo diferente de string retorne uma mensagem de erro pedindo para o usuário digitar somente strings.
- As strings devem ter comprimento maior que 3.

02 - Crie uma função  array com números fornecidos pelo usuário.
Por exemplo:
```javascript
    numeros = [1, 2, 4, 5, 3, 2, 7, 9, 0, 2]
    //total de items 10 (n=10)
```
E retorne o resultado da multiplicação como descrito abaixo:
```javascript
     multiplicacao = numeros[0] * numeros[n-1] //no caso , numeros[0] e numeros[9] multiplicacao = 1*2
    resto = numeros[0]%numeros[n-1] // no caso, numeros[0]%numeros[9] resto = 1%2 
```

03.Crie uma função que receba uma string que pode ser uma das quatro operações básicas da matemática('soma', 'subtração', 'multiplicação' e 'divisão') como primeiro argumento,e o segundo e terceiro como números em que essa operação seja aplicada .

```javascript
    //Exemplo
    funcao('soma', 1, 2)
    //return
    3
```
04. Refaça a questão 03 de modo que as operações básicas sejam funções que serão chamadas dentro da função principal

```javascript
    funcao('soma', 1, 2)

    //soma 
    soma(num1, num2){

    }
    //funcao principal
    funcao(operacao, num1, num2){
        //soma
        soma(num1, num2)
    }
```
05.Crie uma função que adicione números de forma "ilimitada";

06.Crie uma função que calcule o fatorial de um número fornecido como argumento.
Por exemplo:
```javascript 
    fatorial(5) // 5! = 5x4x3x2x1 = 120
```
07. Refaça a questão 04 utilizando Common JS. Você deve criar um arquivo "menu.js" e outro arquivo "operacoes.js" para essa questão.

08. Refaça a questão 04 utilizando ECMAScript Modules(ESM). Você deve criar um arquivo"menu.js" e outro arquivo"operacoes.js" para essa questao.

09. Crie um script que permita salvar usuarios como nome e matrícula e que liste esses usuarios. Use o ESM com um arquivo que guarda os usuarios e outro com as funções de salvar e outra de listar.

