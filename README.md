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

  `docker stop name`  

## Iniciar um container  

  `docker start mongo`  

## remover um container  

  `docker rm mongo`  
