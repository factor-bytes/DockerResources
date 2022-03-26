# Some common docker commands

## Build a docker Image
docker build -t aa-imagename .
  
  
## Prune docker images
docker image prune -a

## Run Docker Compose
Docker-compose up -d

## Stop Containers 
docker-compose stop 

## List all Containers
docker container ls -a


## Stop all containers
docker kill $(docker ps -q)

## Remove all containers
docker rm $(docker ps -a -q)




