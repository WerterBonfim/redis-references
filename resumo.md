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



KEYS nota:*:*
keys nota:*:??????

```

Padroes:
tipo:indentificador:campo

set "nota:10-03-2019
