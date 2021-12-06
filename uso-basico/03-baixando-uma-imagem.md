## Baixando uma imagem. 

Bom, já vimos como fazer isso. Só que agora vamos baixar uma imagem diferente.
Então sem enrolação, vamos lá: 

Digite:

```docker container run debian```


Se você está usando linux ou mac pode rodar o comando: 

```bash --version``` 
```docker container run debian bash --version``` 

o primeiro comando retornará a versão do bash e o segundo retornará também a versão do bash, mas esse bash não é o mesmo que está na sua máquina, você pode ver isso nas versões retornadas. É o bash do debian. 

Mas espera... Então o debian está usando outro terminal? Sim, ele apenas está usando algumas libs e o kernel do seu SO primário e rodando tudo em cima disso.