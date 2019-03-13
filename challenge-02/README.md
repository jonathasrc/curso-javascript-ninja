# Desafio da semana #2

```js
Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.

function sum(arg1,arg2){
  return (arg1 + arg2)
}
// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
let mySum = sum(3,2) + 5
// Qual o valor atualizado dessa variável?
5
// Declare uma nova variável, sem valor.
let newVar
/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
function addValue(arg1){
  newVar = arg1
  return `O valor da variável agora é ${newVar}`
}
// Invoque a função criada acima.
addValue(25)

// Qual o retorno da função? (Use comentários de bloco).
/*VALOR*/

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
function arg(arg1,arg2,arg3){
  error = 'Preencha todos os valores corretamente'

  if(arg1 === undefined || arg2 === undefined || arg3 === undefined)
    return error

  let result = (arg1 * arg2 * arg3) + 2
  return result
}

// Invoque a função criada acima, passando só dois números como argumento.
arg(2,3)
// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).

//Pencha todos os valores corretamente

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
arg(1,2,3)
// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).

// 8

/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
function arg2(arg1,arg2,arg3){
  if ( arg1 == undefined && arg2 == undefined && arg3 == undefined)
    return false
  else if(arg2 == undefined && arg3 == undefined)
    return arg1
  else if(arg3 == undefined)
    return (arg1 + arg2)
  else
    return (arg1 + arg2)/arg3

  return null
}
// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
//arg2(2)
//arg2(1,2)
//arg2(10,10,2)
//arg2()
```
