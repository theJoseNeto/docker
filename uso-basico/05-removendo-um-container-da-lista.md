## Removendo um container

É bem simples. Basta executar: 

```docker container run --rm debian```

Esse comando vai excluir o container da lista mostrada no documento anterior. 
Então se rodarmos ```dokcer container ps -a``` iremos ter a mesma quantidade de containers, não  terá sido adicionado nenhum a mais.

