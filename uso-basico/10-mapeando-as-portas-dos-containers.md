## Mapeando as portas dos containers 

Por enquanto ainda estamos no uso mais básico possível do docker (como sugere o nome da pasta). 
Mas logo nos aprofundaremos nos assuntos. 

Vamos rodar o comando: 

```docker container run -p 8080:80 nginx```. 

A porta `8080` será a porta de onde vamos acessar a porta `80`. Lembra das conecções que falei que os containers devem ter: Aí está. 

Depois de rodar o comando acima, vamos abrir outro terminal (já que o container está funcionando no atual) e digitar: 

`curl http://localhost:8080` ou acessar seu browser e buscar por `http://localhost:8080` você vai ter o retorno da página no nginx



