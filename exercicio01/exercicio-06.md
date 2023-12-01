# Exercício JS 6

## 1. Ceverino tem uma estante com três compartimentos um em cima do outro. Cada compartimento comporta três caixas uma ao lado da outra. As caixas possuem duas características que o Ceverino sempre observa: cor da caixa e a numeração escrita nela. Sabendo disso, escolha uma estrutura de dados para representar a estante de Ceverino e um tipo de dado para representar a caixa.
**Exemplo ilustrativo da estante de Ceverino:**
<div align="center">
    <img title="Exemplo ilustrativo da estante de Ceverino" src="./utils-exe-06/image01-exe-06.png"/>
</div>

## 2. A partir do exercício 1, crie uma função que receba dois parâmetros:
- Estrutura que você escolheu no exercício 1
- Um número que representará o índice do compartimento da estante
## A função deve retornar:
- As informações de todas as caixas que estão no compartimento solicitado

**Exemplo ilustrativo das caixas da estante que serão retornadas, caso o primeira compartimento seja o solicitado:**
<div align="center">
    <img title="Exemplo ilustrativo da estante de Ceverino" src="./utils-exe-06/image02-exe-06.png"/>
</div>

## 3. A partir do exercício 1, crie uma função que receba dois parâmetros:
- Estrutura que você escolheu no exercício 1
- Um número que representará o índice da coluna dos compartimentos da estante
## A função deve retornar:
- As informações de todas as caixas que estão nos compartimentos na coluna solicitada

**Exemplo ilustrativo das caixas da estante que serão retornadas, caso a primeira coluna seja o solicitada:**
<div align="center">
    <img title="Exemplo ilustrativo da estante de Ceverino" src="./utils-exe-06/image03-exe-06.png"/>
</div>

## 4. A partir do exercício 1, crie uma função que receba dois parâmetros:
- Estrutura que você escolheu no exercício 1
## A função deve retornar:
- As informações de todas as caixas que estão na diagonal principal da estante

**Exemplo ilustrativo das caixas da estante que serão retornadas:**
<div align="center">
    <img title="Exemplo ilustrativo da estante de Ceverino" src="./utils-exe-06/image04-exe-06.png"/>
</div>

## 5. A partir do exercício 1, crie uma função que receba dois parâmetros:
- Estrutura que você escolheu no exercício 1
## A função deve retornar:
- As informações de todas as caixas que estão na diagonal secundária da estante

**Exemplo ilustrativo das caixas da estante que serão retornadas:**
<div align="center">
    <img title="Exemplo ilustrativo da estante de Ceverino" src="./utils-exe-06/image05-exe-06.png"/>
</div>

## 6. Crie uma função chamada **uniqueValues** que receba como parâmetro: 
- Uma lista de números
## A função deve retornar:
- A mensagem "O parâmetro deve ser uma lista!", caso o parâmetro **não** seja uma lista
- Uma lista com todos os números **sem** repetições, caso os parâmetros estejam no formato correto
- Uma lista vazia, caso a lista esteja vazia

**Exemplo:**
```JavaScript
const numbers = [1, 2, 3, 3, 2, 4, 0]

console.log(uniqueValues(numbers))
/* resultado no terminal deve ser:
[1, 2, 3, 4, 0]
*/

console.log(uniqueValues([]))
/* resultado no terminal deve ser:
[]
*/

console.log(uniqueValues(2))
/* resultado no terminal deve ser:
O parâmetro deve ser uma lista!
*/
```

## 7. Crie uma função chamada **innerJoin** que receba dois parâmetros: 
- Uma lista de números
- Uma lista de números
## A função deve retornar:
- A mensagem "O primeiro parâmetro deve ser uma lista!", caso o primeiro parâmetro **não** seja uma lista
- A mensagem "O segundo parâmetro deve ser uma lista!", caso o segundo parâmetro **não** seja uma lista
- Uma lista com todos os números que estão em ambas as listas, caso os parâmetros estejam no formato correto
- Uma lista vazia, caso não haja números que estão em ambas as listas

**Exemplo:**
```JavaScript
const numbers1 = [1, 2, 3, 3, 2, 4, 0]
const numbers2 = [1, 2, 3, 5, 10]

console.log(innerJoin(numbers1, numbers2))
/* resultado no terminal deve ser:
[1, 2, 3]
*/

console.log(innerJoin([], numbers2))
/* resultado no terminal deve ser:
[]
*/

console.log(innerJoin(2, numbers2))
/* resultado no terminal deve ser:
O primeiro parâmetro deve ser uma lista!
*/
```

## 8. O código abaixo foi escrito por Ceverino. Sua intenção era mostrar os dados que estão no arquivo [users.csv](./utils-exe-06/users.csv) no terminal. Na máquina do Ceverino, o arquivo que o código está escrito e o arquivo users.csv estão localizados no mesmo diretório. Ao executar o código, aparecia a seguinte mensagem no seu terminal: Promise { \<pending> }. Dito isso, ajude Ceverino a alcançar seus objetivos alterando o que for preciso no código: 
**Código:**
```JavaScript
const fs = require('fs').promises

const usersString = fs.readFile('./users.csv', 'utf-8', 'r')

console.log(usersString)

// ...
```

## 9. A partir do código abaixo e dos arquivos [users.csv](./utils-exe-06/users.csv) e [address.csv](./utils-exe-06/address.csv), desenvolva um algoritmo que imprima no terminal os dados dos usuários e seus respectivos endereços:
**Código:**
```JavaScript
const fs = require('fs').promises

// ...
```
**Exemplo de saída no terminal:**
```cmd
Usuário: Carlos Júnior
Endereço: Av. José Listeu, 24

Usuário: Joao Vitor
Endereço: Rua Teixeira dos Santos, 456

Usuário: Joao Carlos
Endereço: Rua Raimundo Meneguel, 7899

Usuário: Thiago Alves
Endereço: Rua Lenador Lenha Ra, 10
```

***Observação:** tente resolver o problema mantendo a estrutura dos arquivos.*

***Dicas:** pesquise sobre as funções nativas de uma **string**, como por exemplo **split()** e **replace()**. Elas podem te ajudar.*