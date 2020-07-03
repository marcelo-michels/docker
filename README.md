# docker

## Docker Version

  `docker version`

## Listar todos os contaiters que estão rodando 

  `docker ps`

## Listar todos os contaiters que estão parados 

  `docker ps -a`

## Remove todos os containers  

  `docker system prune`  
  `docker container prune`

## Inicia um docker compose file  

  `docker-compose up -d`  

## Para todos os containers que estejam rodando 

  `docker stop $(docker ps -aq)`  

## Parar um container  

  `docker stop <container_id>`  

## Iniciar um container  

  `docker start <container_id>`  

## remover um container  

  `docker rm <container_id>`  

## entrar no terminal de um container

  `docker exec -it <container_id> bash`  
