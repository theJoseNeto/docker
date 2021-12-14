## Rodando um serviço web em background. 

Rodando o docker em background começamos a usar de fato o docker do jeito que ele foi projetado pra usar. 
Então, vamos lá: 

` docker container run -d --name docker-daemon-example -p 8080:80 -v $(pwd)example/html:user/shared/html ngnix`

`-d` vai rodar nosso container no modo daemon
`--name` Já sabemos que é pra renomear 
`-p` Vamos mapear a porta do nosso container 
`-v` Vamos mapear qual volume o diretório ele vai usar.  

Ao rodar esse container ele será executado em background. Se você rodar o comando  `docker container ps` verá que há um  container em execução. 

Caso você queira fazer alguma operação de restartar, iniciar ou parar seu contaiener, você pode usar esse container

`docker container start <container name>` --> Para iniciar o container;
`docker container restart <container name>` --> Para reiniciar o container;
`docker container stop <container name>` --> Para parar o container; 


Outra maneira de controlar seu container é ao invés de passar o nome do container você pode passar o id daquele container no lugar. Exemplo: 

`docker container start Asda31241bxv` --> Para iniciar o container;
`docker container restart Asda31241bxv` --> Para reiniciar o container;
`docker container stop Asda31241bxv` --> Para parar o container; 
