## Reutilização de containers 

Agora que temos um container nomeado por nós, vamos chama-lo com o comando: 

```docker container start -ai meuContainer``` 

Sobre a flag ```-ai``` : Ela seria equivalente a flag ```-it``` e vai abrir o terminal do conatainer selecionado no modo interativo. Lenbra do teste que fizemos para provar que estávamos no mesmo container? Vamos faze ele novamente: 
Após ter aberto o terminal do seu container digite ```touch index.txt``` depois ```ls``` para listar os arquivos do seu container. Você verá que o arquivo está lá. Agora digite ```docker container start -ai meuContainer``` e ```ls```. Viu? seu arquivo ainda está lá. 
