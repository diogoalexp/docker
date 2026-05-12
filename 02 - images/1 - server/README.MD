# Node.js Server

A Node.js application containerized with Docker.

## Getting Started

### Build the Image

```bash
docker build .
```

### Run the Container

Run the image as a container with port mapping:

```bash
docker run -p 3000:80 {IMAGE_ID}
```

**Port mapping:** `-p machinePort:containerPort`
- Maps port 3000 on your machine to port 80 in the container

### Container Management

List running containers:

```bash
docker ps
```

Stop a container:

```bash
docker stop {CONTAINER_NAME}
```

---

## Notes

- Replace `{IMAGE_ID}` with the actual image ID from the build output
- Replace `{CONTAINER_NAME}` with the actual container name from `docker ps`
- Access the server at `http://localhost:3000`