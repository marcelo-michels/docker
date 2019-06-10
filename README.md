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
  `mkdir -p ~/developer/mongodb`  
Fazer download e iniciar a imagem mongo usando um name 'mongo'  
  `docker run --name mongo -d -p 27017:27017 -v ~/developer/mongodb:/data/db mongo`  
Parar o mongo pelo name 'mongo'  
  `docker stop mongo`  
Iniciar o mongo pelo name 'mongo'  
  `docker start mongo`  
remover o contaiter com o mongo pelo name 'mongo'  
  `docker rm mongo`  
