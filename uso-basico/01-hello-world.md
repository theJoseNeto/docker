## Hello world Docker. 

Para prosseguir daqui em diante você deverá ter o <a href="https://www.docker.com/products/docker-desktop">Docker instalado</a> na sua máquina. 

Agora vamos testar. abra o terminal que você geralmente usa e digite: 

```docker```

Isso deve te retornar algo como isso: 

```
Usage:  docker [OPTIONS] COMMAND

A self-sufficient runtime for containers

Options:
      --config string ...

```

Vai retornar muito mais coisa, mas não vou colocar aqu, é só pra você testar.

E agora que seu docker fuciona (ou não, espero que sim), vamos rodar um comando real: 

```docker container run hello-world```

Se você nunca rodou esse comando antes, o ```docker container run``` vai procurar por essa imagem na sua máquina e não  vai encontrar. Então a imagem ```hello-world```será baixada. 

Ao ter rodado esse comando, será retorada uma mensagem com uma explicação do que acabou de acontecer com seu docker. Algo como: 

```
Hello from Docker!
This message shows that your installation appears to be working correctly.

```

Basicamente ele explica que o docker client "chamou" o docker daemon, que é o sistema que o docker usa para se comunicar com  o docker hub onde foi encontrada a imagem "hello-world" e aí o docker daemon cria um novo container baseado nessa imagem.  

Ele explica mais alguamas coisinhas, mas por enquanto vamos permanecer no raso, logo logo iremos nadas em águas mais profundas. 


