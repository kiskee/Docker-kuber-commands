#Initial commands for docker

docker run --imageName
docker stop --
docker kill --
docker create --
docker start --
docker ps --
docker system prune -a

###redis

docker run redis

docker exec -it (into container in text) <container-id> <command>

###entrar a la terminal del contenedor o el shell
docker exec -it <container-id>

####para salir de la consola de un container
crt+d

#tags
docker build -t daniel/redis:latest .