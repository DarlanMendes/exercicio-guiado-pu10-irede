# Exercício JS 4

***Observação:** para os exercícios propostos, **não** utilize funções nativas do JavaScript como Array.find(), Array.filter(), etc.*

## 1. Crie uma função chamada **findUserById** que receba dois parâmetros: 
- Uma lista de objetos que representarão usuários
- Um número que representará o id do usuário
## A função deve retornar:
- A mensagem "O primeiro parâmetro deve ser uma lista!", caso o primeiro parâmetro **não** seja uma lista
- A mensagem "O segundo parâmetro deve ser um número!", caso o segundo parâmetro **não** seja um número
- O usuário pesquisado, caso exista
- Null, caso **não** exista

**Exemplo:**
```JavaScript
const users = [
    {
        id: 1,
        name: 'Carlos Júnior',
        age: 26
    },
    {
        id: 2,
        name: 'Ceverino Cordeiro',
        age: 70
    }
]

console.log(findUserById(users, 2))
/* resultado no terminal deve ser:
{
    id: 2,
    name: 'Ceverino Cordeiro',
    age: 70
}
*/

console.log(findUserById(users, 5))
/* resultado no terminal deve ser:
null
*/

console.log(findUserById(users, '2'))
/* resultado no terminal deve ser:
O segundo parâmetro deve ser um número!
*/
```

## 2. Crie uma função chamada **filterProductByName** que receba dois parâmetros: 
- Uma lista de objetos que representarão produtos
- Uma string que representará o nome do produto
## A função deve retornar:
- A mensagem "O primeiro parâmetro deve ser uma lista!", caso o primeiro parâmetro **não** seja uma lista
- A mensagem "O segundo parâmetro deve ser uma string!", caso o segundo parâmetro **não** seja uma string
- Uma nova lista com o(s) produto(s) pesquisado(s), caso exista(m)
- Uma nova lista vazia, caso **não** exista

**Exemplo:**
```JavaScript
const products = [
    {
        id: 1,
        name: 'Jogo de Panelas',
        price: 54.59
    },
    {
        id: 2,
        name: 'Chocolate L',
        price: 14.99
    },
    {
        id: 3,
        name: 'Sabão Lili'
        price: 29.99
    }
]

console.log(filterProductByName(products, 'cho'))
/* resultado no terminal deve ser:
[
    {
        id: 2,
        name: 'Chocolate L',
        age: 14.99
    }
]
*/

console.log(filterProductByName(products, 'Arroz'))
/* resultado no terminal deve ser:
[]
*/

console.log(filterProductByName(products, 2))
/* resultado no terminal deve ser:
O segundo parâmetro deve ser uma string!
*/
```

## 3. Crie uma função chamada **mapProductsRemoveId** que receba como parâmetro: 
- Uma lista de objetos que representarão produtos
## A função deve retornar:
- A mensagem "O parâmetro deve ser uma lista!", caso o parâmetro **não** seja uma lista
- Uma nova lista com o(s) produto(s) **sem** a propriedade id, caso a lista tenha produtos
- Uma nova lista vazia, caso a lista esteja vazia

**Exemplo:**
```JavaScript
const products = [
    {
        id: 1,
        name: 'Jogo de Panelas',
        price: 54.59
    },
    {
        id: 2,
        name: 'Chocolate L',
        price: 14.99
    },
    {
        id: 3,
        name: 'Sabão Lili'
        price: 29.99
    }
]

console.log(mapProductsRemoveId(products))
/* resultado no terminal deve ser:
[
    {
        name: 'Jogo de Panelas',
        price: 54.59
    },
    {
        name: 'Chocolate L',
        price: 14.99
    },
    {
        name: 'Sabão Lili'
        price: 29.99
    }
]
*/

console.log(mapProductsRemoveId([]))
/* resultado no terminal deve ser:
[]
*/

console.log(filterProductByName(2))
/* resultado no terminal deve ser:
O parâmetro deve ser uma lista!
*/
```

## 4. Crie uma função chamada **sumProductsPrice** que receba como parâmetro: 
- Uma lista de objetos que representarão produtos
## A função deve retornar:
- A mensagem "O parâmetro deve ser uma lista!", caso o parâmetro **não** seja uma lista
- O resultado da soma dos preços dos produtos, caso a lista tenha produtos
- O valor 0, caso a lista esteja vazia

**Exemplo:**
```JavaScript
const products = [
    {
        id: 1,
        name: 'Jogo de Panelas',
        price: 54.59
    },
    {
        id: 2,
        name: 'Chocolate L',
        price: 14.99
    },
    {
        id: 3,
        name: 'Sabão Lili'
        price: 29.99
    }
]

console.log(sumProductsPrice(products))
/* resultado no terminal deve ser:
99.57
*/

console.log(sumProductsPrice([]))
/* resultado no terminal deve ser:
0
*/

console.log(sumProductsPrice(2))
/* resultado no terminal deve ser:
O parâmetro deve ser uma lista!
*/
```