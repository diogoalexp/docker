# Docker & Kubernetes Learning

Learn practical Docker and Kubernetes commands and best practices.

---

## Important Commands

### Build

Build a Docker image from a Dockerfile:

```bash
docker build .
```

### Run and Start

#### Create and Run a Container

Run an image as a container with port mapping:

```bash
docker run -p 3000:3000 {IMAGE_ID}
```

**Port mapping:** `-p machinePort:containerPort`

#### Detached Mode

Run a container in the background (no console logs displayed):

```bash
docker run -p 3000:3000 -d {IMAGE_ID}
```

#### Restart an Existing Container

Restart a previously created container without creating a new image:

```bash
docker start {CONTAINER_NAME}
```

### List Containers

List running containers:

```bash
docker ps
```

List all containers (running and stopped):

```bash
docker ps -a
```

### Stop

Stop a running container:

```bash
docker stop {CONTAINER_NAME}
```

---

### Remove Containers

Remove container by name:

```bash
docker rm {CONTAINER_NAME} {CONTAINER_NAME}
```

remove all containers:

```bash
docker rm *
```

Remove images by id:

```bash
docker rmi {IMAGE_ID}
```

## Useful Commands

### Attach Terminal to Container

Attach your terminal to a running container:

```bash
docker attach {CONTAINER_NAME}
```

---

## Important Notes

⚠️ **Every time you make a code change, you must build a new image for the changes to be reflected in the container.**

- Replace `{IMAGE_ID}` with the actual image ID from the build output
- Replace `{CONTAINER_NAME}` with the actual container name from `docker ps`
