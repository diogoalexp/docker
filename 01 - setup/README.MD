Build the image
> docker build .

Run the Image as a container in a speficic port
-p machinePort : containerPort
> docker run -p 3000:3000 {IMAGE_ID}

List the running containers
> docker ps

Stop the containers
> docker stop {CONTAINER_NAME}