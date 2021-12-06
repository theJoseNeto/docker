## Nomeação de containers. 

Nesse tutorial vamos aprender a nomear containers, para aprendermos também a reutilizar os containers. Como citado antes o comado  ```run``` sempre cria novos containers, e não sei e você percebeu, mas esse containers recebem nomes aleatórios. Vamos checar isso com o comando ```docker ps -a```. Se você prestar atenção na coluna "NAMES" vai ver que tem alguns nomes aleatórios. 
Agora vamos aprender a nomear nossos containers. 

```docker container run --name nomeDoSeuContainer -it debian bash```

Agora vamos sair do nosso container com o comando ```exit```, e em seguida vamos tentar rodar o mesmo comando que fizemos antes de ```exit```.

Retorno no terminal: 


<code>

docker: Error response from daemon: Conflict. The container name "/meuContainer" is already in use by container "...". You have to remove (or rename) that coontainer to be able to reuse that name. See "docker run --help". 

</code>


Se você rodar o comando ```docker container ps -a``` irá ver que seu container está na lista da coluna "NAME".

