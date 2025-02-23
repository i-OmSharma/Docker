* docker run -p HOST_PORT:CONRTAINER_PORT IMAGE_NAME

by default containers have prots binded to them, all of docker container file system seperate to them these files are seperate from the host machine.
same like that the ports of containers are different from the host machine. 

* docker run -p HOST_PORT:CONRTAINER_PORT IMAGE_NAME
using this command we can bind the host port to the container port, and this mapping is called PORT BINDING.

We can't allocate same port to different containers, the actaul or the host machines different port should be used for binding.