## Um container totalmente isolado...? 

Acho que essa não é uma boa ideia, segundo o que estou estudado enquanto crio esse texto. 

Isolar totalmente um container torna ele um tanto quanto inútil. Por que se você cria um container paras as partes da sua aplicação mas isola eles completamente, de quê ele serve?
Então por isso temos que isolar as partes da aplicação, mas podemos expor uma porta, pra que alguém ou você  consiga acessar um serviço que está em execução dentro do container, ou compartilhar uma pasta entre o container e a maquina host, copiar arquivos do container para a máquina host e vise versa e por ultimo, a comunicação  entre os próprios containers da sua aplicação: 
Um para o backend que se comunica com o frontend e a base de dado. 

 - <i>"Então eu não posso criar um container totalmente isolado?"</i>

Sim, pode. Mas, entretatanto, contudo, todavia, você não vai conseguir explorar todas as capacidades e funcionalidades do docker da mesma maneira. 