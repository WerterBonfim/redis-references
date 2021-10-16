```bash

# iniciar o docker
docker container run --name redis --rm -h "redis.docker" -p 6379:6379 --memory="1g" -it redis:6.2.5-alpine

# entrar dentro do container
docker container exec -it redis sh

# acessando o redis-cli
redis-cli



```

```bash

# insert

set "usuarios_online" 42

# obter
get usuarios_online

# atualizar
set "usuarios_online" 43

# deletar

del "usuarios_online"

# ver todas as chaves
keys *


set "nota:14-04-2019:matematica" 8.5
set "nota:20-06-2019:historia" 9.5
set "nota:20-06-2019:historia" 9.5
set "nota:22-06-2019:fisica" 6.5

# retonar as chavas que contem notas
keys nota*

# padrões de pesquisa

keys nota:*-06*

KEYS nota:*:*
keys nota:*:??????

```

Padroes:
tipo:indentificador:campo

set "nota:10-03-2019
