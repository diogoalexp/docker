# docker
Learn practices about docker and kubernets

Build the image
> docker build .

Create and Run the Image as a container in a speficic port
-p machinePort : containerPort
> docker run -p 3000:3000 {IMAGE_ID}

deatched version (no console and logs)
> docker run -p 3000:3000 -d {IMAGE_ID}

Restart an existing container (without creating a new image)
> docker start {CONTAINER_NAME}

Attach the terminal to a running container
>docker attach CONTAINER

List the running containers
> docker ps

List all containers
> docker ps -a

Stop the containers
> docker stop {CONTAINER_NAME}

## changes
Everytime you need to make a code change is necessary to build a new image
