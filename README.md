# Docker

## Build a Docker Image
docker build -t gtxvii/myapp:1.0 . (. is the path to the current directory)

## Run Docker Image
docker run sha256:6428e5... (sha or image name)

## Run with port forwarding
docker run -p 5000:8080 sha256:6428e5…  (sha or image name)

## Show all running containers
docker ps

## Stop a container
docker stop sha:123....  (sha or image name)

## Push to Dockerhub
docker push gtxvii/nameofyourapp:1.0

## Create a Volume
docker volume create shared-data<br>docker run –mount source=shared-data,target=/stuff  sha256:64…

### Local dir volume
docker run --mount type=bind,source=/path/on/host,target=/path/in/container sha256:64…

## Compose multiple containers
docker-compose up –build -d<br>docker-compose down
