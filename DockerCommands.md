# Some common docker commands

## Build a docker Image
docker build -t aa-imagename .
  
  
## Prune docker images
```
docker image prune -a
```

## Run Docker Compose
Docker-compose up -d

## Container Status
Docker-compose ps

## Stop Containers 
docker-compose stop 

## List all Containers
docker container ls -a


## Stop all containers
docker kill $(docker ps -q)

## Remove all containers
docker rm $(docker ps -a -q)

-------------------------------------------------


## How to SSH into a running container
1. Get running container name  - docker ps or docker-compose ps
2. Use the command docker exec -it <container name> /bin/bash to get a bash shell in the container
