Find out where Docker-compose file is located

Use the IDE or  Execute forllowing


`ls 
 cd pitshop-microservices/src
`{{execute}}

Go to the folder where Docker compose file 

Run `docker-compose build`{{execute}}

It will take time once it is completed rum docker images to see  the result

`docker  images`{{execute}}

create Volumes for sql server and rabbitmq
`docker volume create --name=sqlserverdata 
docker volume create --name=rabbitmqdata' {{execute}}


Run all the services execute docker-compose up

`docker-compose up -d`{{execute}}