### Docker run - To start a container

docker run nginx [runs instance of nginx if not found locally downloads from dockerhub and runs it]

### Docker ps  - To list all containers in in the local machine

docker ps outpts only active/running containers
docker ps -a lists all containers

### Docker stop [containerID/containerName]
docker stop   4347004047ad

or 

docker stop hello-world

### docker rm - remove container from the local machine

docker rm hello-world

removes only the container and not the image from which it was created. It is possible to create multiple container from same image. For eg. a image having wordpress installation can be used to create multiple container so that we have multiple wordpress site.

### docker images - list all available images.

docker images

### docker rmi [iamgeID/imageName] - Make sure that all dependant container created from this image should be deleted before removing the image

docker rmi hello-world

### docker pull [imageName] - downloads the image and does not start a container by default as docker run commands

docker pull hello-world

### docker exec - To execute command inside a docker container

docker exec [running-container-name]  cat /etc/hosts


### docker run -d [imageName]

docker create a container with the image. the -d will run the conatiner in the background.

to bring docker container running in background to foreground run, 

##### docker attach [containerID]

### docker run ubuntu
will create latest ubuntu version [as on 2020 it is 20.04 LTS]

if you want to create ubuntu version 18.04

##### docker run ubuntu:18.04

docker commands use TAG and 18.04 is version TAG






