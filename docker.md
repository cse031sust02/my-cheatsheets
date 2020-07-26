## Terminology :

#### Dockerfile :
A Dockerfile is a blueprint for building Docker images. It is simply a text file which contains the build instructions to build the image.

#### Image : 
Docker images are executable packages that include everything needed to run an application — the code, a runtime, libraries, environment variables, and configuration files. We can create our own image from scratch or can use iamges built by others.

#### Container : 
A Docker container is a running instance of a Docker image. We can think of a Docker container as a Object in OOP world which was created by it's Image(Class).* A container can expose ports and volumes to interact with other containers or/and the outer world. 

> *It's not an accurate analogy but good to understand in this way. 

#### Volume : 
Volumes are designed to persist data and share between containers. Volumes are independent of the container’s lifecycle.

#### Docker Compose : 
Docker Compose is a tool for defining and running multi-container Docker applications. The docker-compose.yml allows us to configure all our application's services in one place and start them all with a single command.

#### Docker Hub :
Docker Hub is the default public registry which is managed by Docker (the company). Anybody can build and host their Docker images on Docker Hub, we can find images for most of the apps and linux distros we need there. It's like github for docker images.

> In short, Docker images hold the snapshot of the Dockerfile, and the Docker container is a running implementation of a Docker image based on the instructions contained within that image. All of this is taken care of by the Docker Engine.

## Commands :

#### - download images to our computer
----
```
$ docker pull <image-name>
```

#### - builds an image from a Dockerfile
----
```
$ docker build <path>
```

#### - docker images that have been downloaded/built
----
```
$ docker images
```

#### - removes one or more images
----
````
$ docker rmi <image-name>
````

#### - run a container
----
````
$ docker run <image-name>
````

#### - list of containers
----
````
$ docker ps      # list out the running containers only
$ docker ps -a   # list out all contaiers (including  the stopped containers)
````

#### - enter the bash of a container
----
````
$ docker exec -it <container-id-or-name> bash
````

#### - stop containers
----
````
$ docker stop <container-id-or-name>
````

#### - removes one or more containers
----
````
$ docker rm <container-id-or-name>
````
