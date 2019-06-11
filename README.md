# docker

#### Docker Version
  `docker version`

#### Listar todos os contaiters que estão rodando 
  `docker ps`

#### Listar todos os contaiters que estão parados 
  `docker ps -a`

#### Limpar o docker
  `docker system prune`  
  `docker container prune`
  
#### Ubuntu
Criar um container que roda a partir da imagem do ubuntu  
  `docker run ubuntu`

Criar um container que roda a partir da imagem do ubuntu e executa um comando dentro do container  
  `docker run ubuntu echo "Ola Mundo"`
 
Criar um container que roda a partir da imagem do ubuntu e abre o terminal do container  
  `docker run -it ubuntu`
 
#### Mongo
Criar uma pasta para guardar os dados do banco  
  `mkdir -p ~/developer/docker/mongodb`  
Fazer download e iniciar a imagem mongo usando um name 'mongo'  
  `docker run --name mongo -d -p 27017:27017 -v ~/developer/docker/mongodb:/data/db mongo`  
Parar o mongo pelo name 'mongo'  
  `docker stop mongo`  
Iniciar o mongo pelo name 'mongo'  
  `docker start mongo`  
remover o contaiter com o mongo pelo name 'mongo'  
  `docker rm mongo`  

#### Postgres
Criar uma pasta para guardar os dados do banco  
  `mkdir -p ~/developer/docker/postgres/12`  
Fazer download e iniciar a imagem postgres:12 usando um name 'postgres12'  
  `docker run --name postgres12 -d -p 5412:5432 -v ~/developer/docker/postgres/12:/var/lib/postgresql/data -e POSTGRES_PASSWORD=123456 -d postgres:12`  
Parar o postgres pelo name 'postgres12'  
  `docker stop postgres12`  
Iniciar o postgres pelo name 'postgres12'  
  `docker start postgres12`  
remover o contaiter com o postgres pelo name 'postgres12'  
  `docker rm postgres12`  
