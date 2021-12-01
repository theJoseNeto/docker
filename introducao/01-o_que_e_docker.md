# O que é docker?

Nesse primeito momento vamos falar os conceitos mais básicos do que é docker.

## O que não é docker

Não é uma sitema de virtualização como o sistema de uma VM (virtual machine).


## Então ele é...


Ele é uma engine que administra containers. 
Os containers são processos que literalmente segregam nosso projeto para que consigamos rodar nosso projeto da forma mais controlado possível. 

## Por que não é a mesma coisa que uma VM: 

Apesar de um pouco parecidos (e as vezes até são postos como a mesma coisa), são coisas totalmente diferentes. Já que a VM é um sistema totalmente á parte do sistema que roda na máquina host (sua máquina). 
O container mesmo segregando o projeto, ele ainda depende de certos arquivos, binários e o kernel. O que torna ele mais rápido, já que parte do que ele precisa já está alí. E com a VM é diferente, ela tem que recarregar tudo sempre que necessário.

## O que o docker usa ali por baixo dos panos?

Basicamente ele utiliza os serviços do LXC (linux container). 
Você pode ler mais sobre isso <a href="#">aqui</a>.

## Docker e algumas de suas vantagens. 

Não sou do time que é fã de tecnologia, mas admito que o docker se destaca em vários quesitos. Algumas das vantagens é que o docker nos permite controlar inúmeras coisas dentro do nosso container. Entre elas: Quantidade de memória que aquele container vai utilizar, quantidade de CPU que será consumida. Temos mais coisas que podemos falar, mas essa é apenas uma introdução. 



