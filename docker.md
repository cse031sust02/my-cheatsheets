download images to our computer
----
```
$ docker pull <image-name>
```

builds an image from a Dockerfile
----
```
$ docker build <path>
```

docker images that have been downloaded/built
----
```
$ docker images
```

removes one or more images
----
````
$ docker rmi <image-name>
````

run a container
----
````
$ docker run <image-name>
````

list of containers
----
````
$ docker ps
````

enter the bash of a container
----
````
$ docker exec -it <container-id-or-name> bash
````

stop containers
----
````
$ docker stop <container-id-or-name>
````

removes one or more containers
----
````
$ docker rm <container-id-or-name>
````