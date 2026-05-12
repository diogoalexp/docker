# Python Random Number Generator

A simple Python application containerized with Docker.

## Getting Started

### Build the Image

```bash
docker build .
```

### Run the Container

Run the image as a container in interactive mode (no ports needed):

```bash
docker run -it {IMAGE_ID}
```

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
- The `-it` flag runs the container in interactive mode with a terminal