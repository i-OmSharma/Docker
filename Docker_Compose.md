Docker Compose is a tool for defining and running multi-container applications. 

Docker Compose Commands:
- docker compose -f fileName.yaml up -d
- docker compose -f fileName.yaml down

in docker file yaml we dont define the network as we use to do in the terminal.
here the yaml file creates a default network, and it will run all the containers inside the network.

we dont need to create a network docker compose does it automatically.