## Docker Image

Docker Image helps us to create multiple containers.
Resources are being used by the containers not the images.
Docker Image is static snapshot of what the local development should look like. 

* docker images: for listing docker images.  
* docker ps: listing running containers. 
* docker ps -a: listing all the available containers(both running and stopped).


* docker pull <image_name> --> Pulls an image from Docker Hub to your local machine.
* docker run <image_name> --> Creates a container from the image and runs it. If the image is not available locally, it will first pull it from Docker Hub.
* docker start <container_id_or_name> --> is used to start a stopped container by referring to the container ID or name, not the image name.
* docker stop <container_id_or_name> --> Stops a running container.


* docker run -d is used for detached mode.
* docker run -e is used for the enviroment setup .
* docker run -d -e MYSQL_ROOT_PASSWORD=root mysql --> is used setup env.
eg: like mysql pass.
* docker run -d -e MYSQL_ROOT_PASSWORD=root --name NAME_UR_CONTAINER mysql --> u can name anything u want,using name.


## Layers

Base Layer --> layer 1 --> layer 2 --> Container

Base + 1, 2 , .. layers are read only layers, immutable in nature.
the Container is layer is the where we can make changes.
* When we create  a new container, a new writable layer(called container layer) is added on top of underlaying layers.  