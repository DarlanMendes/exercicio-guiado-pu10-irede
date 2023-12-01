# Mini projeto JavaScript

## Objetivo
O objetivo desse projeto é praticar o conteúdo visto até então sobre a linguagem de programação JavaScript. Além de construir um programa de gerenciamento de pessoas.

## Detalhes
Imagine que você possua uma lista de pessoas com as seguintes informações de cada uma delas: **name**, **email** e **phone**. Além disso, a informação do **email** é única, ou seja, não existe duas ou mais pessoas com o mesmo email. Sua tarefa é desenvolver um programa que gerencie essa lista e use o terminal como forma de interface para que o usuário interaja. O gerenciamento consiste em o usuário conseguir, *via terminal*, **listar**, **adicionar**, **remover**, **editar** e **encontrar** pessoas na lista.

***Observação:** a priore, não se preocupe com a persistência dos dados.*

## Requisitos:
1. A estrutura do seu projeto deve ter, no mínimo, dois arquivos: **main.js** e **utils.js**. O arquivo **main.js** deve conter o seu programa principal. Já o arquivo **utils.js** deve conter as funções utilitárias do seu programa.

2. Seu programa deve conter uma interface via terminal com o usuário. A interface deve reaparecer sempre que uma operação for finalizada, exceto se a operação for relacionada ao encerramento do programa. Na interface deve conter descrito as operações que o seu programa possui e como executá-las. Segue um exemplo meramente **ilustrativo** abaixo:
```cmd
1 - List people
2 - Add one people
3 - Exit
```

3. Seu programa deve conter, no mínimo, as seguintes operações: **listar**, **adicionar**, **remover**, **editar** e **encontrar** pessoas na lista. Além disso, seu programa deve conter uma operação que o encerre e libere o terminal.

***Observação:** ao efetuar as operações **remover**, **editar** ou **encontrar**, a escolha do atributo que irá identificar o usuário da operação é sua. Só não esqueça que apenas o atributo **email** é único.*

## Requisito Bônus:
1. Adicione persistência de dados no seu programa utilizando arquivo **.CSV** ou **.TXT**.