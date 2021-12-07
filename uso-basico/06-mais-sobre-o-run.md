## Mais sobre o comando run. 

Não me recordo se já citei antes, mas o  comando run sempre cria um novo container assim que você chama ele. Pra ver isso de forma interativa vamos executar o run com a tag ```-it``` O "i" é o modo iterativo e o "t" é pra chamar o terminal, ou seja, vamos rodar o terminal dentro do container no modo iterativo. Ficará assim: 

```docker container run -it debian```

Abra outro (Não precisa fechar o terminal onde você statou seu container) terminal e rode o comando ```docker container ps``` novamente e você verá que agora há um container rodando e é justamente o debian. 

Pra provar que o ```run``` cria novos aquivos, abra o terminal onde deixou rodando seu container e digite: ``touch index.txt``. Isso deve ter criado um arquivo de texto no seu container. Para testar se esse arquivo foi criado: ```ls index.txt``` ainda dentro do terminal que pertence ao container, e isso deve ter te retornado o arquivo. 

Agora vamos no outro terminal e rodar o comando 
````docker container run debian````
````docker container run -it debian```` 

e fazer o mesmo processo: 

```touch outro_nome.txt```
 ```ls```

 isso listará todos os documentos do container. Se você perceber index.txt não está nessa lista. Ou seja, estamos em outro container.

 






