# Docker Command Cheat Sheet

## Run a container

docker run [image] [command]

docker run -it [image] [command]

docker run -p [port:image-port] [image]

docker run -P [port:image-port] (for dynamic port)

docker run -d -p [port:image-port] [image]

## Manipulate containers

docker ps [-a]

docker start [ai] | stop[container-id | container-name]

docker rm [container-id | container-name]

docker rm -f [container-id | container-name]

docker rm -f $(docker ps -aq) // delete all containers

docker logs [container-id | container-name]

docker attach [container-id | container-name]

docker commit -m "message" [image-id-to-commit] [name]
