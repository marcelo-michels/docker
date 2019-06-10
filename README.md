# docker

#### Docker Version
  `docker version`

#### Listar todos os contaiters que estão rodando 
  `docker ps`

#### Listar todos os contaiters que estão parados 
  `docker ps -a`

#### Ubuntu
Criar um container que roda a partir da imagem do ubuntu<br/>
  `docker run ubuntu`

Criar um container que roda a partir da imagem do ubuntu e executa um comando dentro do container<br/>
  `docker run ubuntu echo "Ola Mundo"`
 
Criar um container que roda a partir da imagem do ubuntu e abre o terminal do container<br/>
  `docker run -it ubuntu`
 
