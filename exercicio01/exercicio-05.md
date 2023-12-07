# Exercício 05 - Callbacks e High Order Functions

01 - Crie uma função que receba um array de números e um função de callback. A função de callback deve filtrar os números passados do array e devolver somente os números positivos.
Por exemplo:
```javascript
    let numeros=[-2,3,0,4,2-1,-4,8]
    let numerosPares = funcaoPrincipal(numeros, funcaoCallback)
    numerosPares ===> [3,2,8]
```
02 - Crie uma função que receba um array de objetos de compra , um array de objetos de produto e uma função de callback.A função de callback deve verificar a identificação dos produtos presentes no objeto da compra e criar um novo objeto que substitua o identificador pelo objeto do produto.
<br/>
Por exemplo:
```javascript
    let produtos =[
        {id:1, nome:"Traquinas", peso:"500g"},
        {id:2, nome:"Negresco", peso:"300g"},
        {id:3, nome:"Floresta Negra", peso:"370g"}
        ]
    let compras=[
        {id:1, produto_id:1, qtd:3},
        {id:2, produto_id:2, qtd:4}
        ]
    let comprasMapeadas = funcao(compras, produtos, mapeaCompra)

    comprasMapeadas ===> [
        {id:1, produto:{id:1, nome:"Traquinas", peso:"500g"}, qtd:3},
        {id:2, produtos:{id:2,nome:"Negresco", peso:"300g"}, qtd:4}
    ]
```


03 - Crie um função que receba um array de 10 números e faça o somatório dos números ímpares. (Utilize HOF)
Por exemplo:
```javascript
    let numeros=[0, 2, 1, 5, 7, 0, 2, 21, 1, 3]
    //Números a serem somados 1, 5, 7, 21, 1,3 
    let resultado = funcao(numeros)
    resultado ==> 38
```
04 - Refaça a questão 03 utilizando o método reduce( ).


<br/>


05 - Crie uma função que receba um array com objetos que contêm informações de um usuário e retorne um array que contenha somente os nomes dos usuários inadimplentes.
Por exemplo:
```javascript
    let usuarios = [
        {id:1, nome:"Fulano de Tal",pagamento:"pendente"},
        {id:2, nome:"Ronaldo Nazário",pagamento:"pago"},
        {id:3, nome:"Michael Jordan",pagamento:"pago"},
        {id:4, nome:"Maria Rios",pagamento:"pago"},
        {id:5, nome:"Julia Sousa",pagamento:"pago"},
        {id:6, nome:"José Neymar",pagamento:"pendente"},
        {id:7, nome:"Mariana Riacho",pagamento:"pago"},
        {id:8, nome:"Fabiana Beatriz",pagamento:"pendente"},
    ]
    let inadimplentes = selecionaInadimplentes(usuarios)
    inadimplentes ===> ["Fulano de Tal","José Neymar","Fabiana Beatriz"]
```  