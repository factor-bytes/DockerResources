# Some common docker commands

## Build a docker Image
```
docker build -t aa-imagename .
```

## List all docker Images
```
docker image list
```

## Prune all docker images
```
docker image prune --all
```

## Run Docker Compose
```
Docker-compose up -d
```
## Container Status
```
Docker-compose ps
```

## Stop Containers 
```
docker-compose stop 
```

## Stop specific container 
```
docker stop <containerName>
```
```
docker kill <containerName>
```

## List all Containers
```
docker container ls -a
```

## Stop all containers
```
docker kill $(docker ps -q)
```

## Remove a containers
```
docker rm <containerName>
```

## Remove all containers
```
docker rm $(docker ps -a -q)
```

## Tail a container log
```
docker logs --follow <containerName>
```
-------------------------------------------------


## How to SSH into a running container
1. Get running container name  - docker ps or docker-compose ps
2. Use the command below to get a bash shell in the container
```
docker exec -it <container name> /bin/bash
```
