## Mapeamento de diretórios ou volumes de um container. 

Para essa parte não vamos ficar apenas no terminal. Vamos criar um diretorio. 

Você pode usar o `mkdir nomeDoDiretorio` ou criar usando o modo convencional que é `clicar com o botão direito em cimma de uma pasta qualquer > criar nova pasta > nomear pasta > enter`

Nesse caso vou criar uma pasta para esse tutorial e deixar aqui nesse diretório do repositório caso você queira ver. 
Voce pode acessa-lo clicando <a href="./11-example">aqui</a>

Agora vamos rodar um container e mapear a porta `8080` pra ele e usar a flag `-v` para mapear um volume, q

`docker container run -p 8080:80 -v $(pwd)/not-found/usr/share/nginx/html nginx`

