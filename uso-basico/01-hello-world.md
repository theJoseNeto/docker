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

### O que o ```docker container run``` faz: 

Ele busca uma imagem, se ela não existir ele a baixa e a executa dentro do container. E agora se você rodar os comando novamente (com o nome da imagem após o "run") ele terá feito o cache dessa imagem na máquina onde o container foi criado e nem sequer vai carregar mais nada, apenas "rodar" o container com a imagem. Então o comando run ao ser chamado faz o "docker image pull" que o comando para fazer o pull de uma imagem, também roda o comando "docker container create", que eu nem preciso falar muito sobre ele já que o nome é auto explicativo




