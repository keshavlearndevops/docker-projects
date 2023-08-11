# Docker Cheat Sheet 🐳

## Docker Basic Commands 🚀

| Command                          | Description                                 |
|----------------------------------|---------------------------------------------|
| `docker version`                 | Display Docker version information          |
| `docker info`                    | Display system-wide Docker info             |
| `docker pull <image>`            | Download an image from Docker Hub           |
| `docker images`                  | List all local images                       |
| `docker ps`                      | List running containers                     |
| `docker ps -a`                   | List all containers (including stopped)     |
| `docker run <image>`             | Create and start a container                |
| `docker start <container>`       | Start a stopped container                   |
| `docker stop <container>`        | Stop a running container                    |
| `docker restart <container>`     | Restart a running container                 |
| `docker exec -it <cont> <cmd>`   | Run command in a running container          |
| `docker rm <container>`          | Remove a stopped container                  |
| `docker rmi <image>`             | Remove an image                            |
| `docker logs <container>`        | View logs from a container                 |
| `docker build -t <name> <path>`  | Build an image from a Dockerfile           |

## Dockerfile Commands 🏗️

| Command                          | Description                                 |
|----------------------------------|---------------------------------------------|
| `FROM`                           | Set base image for subsequent commands     |
| `RUN`                            | Execute command during image build          |
| `COPY` or `ADD`                  | Copy files from host into the image         |
| `WORKDIR`                        | Set working directory                       |
| `ENV`                            | Set environment variables                   |
| `EXPOSE`                         | Declare open ports at runtime               |
| `CMD`                            | Specify default container command           |
| `ENTRYPOINT`                     | Configure entry point for the container    |
| `VOLUME`                         | Create mount point for external volumes    |
| `USER`                           | Set user for subsequent commands            |
| `LABEL`                          | Add metadata to the image                   |

## Docker Compose Commands 🛠️

| Command                          | Description                                 |
|----------------------------------|---------------------------------------------|
| `docker-compose up`              | Create and start containers                |
| `docker-compose down`            | Stop and remove containers                 |
| `docker-compose build`           | Build or rebuild services                  |
| `docker-compose ps`              | List running containers                    |
| `docker-compose logs`            | View output logs from containers           |
| `docker-compose exec <svc> <cmd>`| Run cmd in a running container            |
| `docker-compose stop`            | Stop services                               |
| `docker-compose start`           | Start services                              |

## Docker Volumes Commands 📦

| Command                          | Description                                 |
|----------------------------------|---------------------------------------------|
| `docker volume create <name>`    | Create a named volume                      |
| `docker volume ls`               | List all volumes                           |
| `docker volume inspect <name>`   | Display detailed volume info               |
| `docker volume ls -q`            | List only volume names/IDs                 |
| `docker volume prune`            | Remove all unused volumes                  |
| `docker volume rm <name>`        | Remove a specific volume                   |
| `docker volume create --driver <name>` | Create a volume with driver            |
| `docker run -v <vol>:<cont_path> <img>` | Mount volume in container            |
| `docker run -v <host>:<cont_path> <img>`| Mount host dir in container         |
| `docker run -v <vol>:/data <img>`| Mount volume at /data in container         |
| `docker run --mount src=<vol>,target=<cont_path> <img>`| Alt. syntax |
| `docker volume create --label <k>=<v> <name>`| Create labeled volume               |
| `docker volume prune --filter "label=<k>=<v>"`| Prune volumes based on label    |

## Docker Networking Commands 🌐

| Command                          | Description                                 |
|----------------------------------|---------------------------------------------|
| `docker network create <name>`   | Create a custom network                    |
| `docker network ls`              | List all networks                          |
| `docker network inspect <name>`  | Display detailed network info              |
| `docker network connect <net> <cont>` | Connect container to network           |
| `docker network disconnect <net> <cont>` | Disconnect container                  |

---

Do check out the following blogs to understand the commands more:

1. [Docker for DevOps Engineers](https://keshavbathla.hashnode.dev/docker-for-devops-engineers)
2. [Docker Project for DevOps Engineers](https://keshavbathla.hashnode.dev/docker-project-for-devops-engineers)
3. [Mastering Docker Compose: Building Beautiful Two-Tier Projects and Beyond](https://keshavbathla.hashnode.dev/mastering-docker-compose-building-beautiful-two-tier-projects-and-beyond)
4. [Deep Dive into Docker: Unveiling Containerization, Networking, and Volumes](https://keshavbathla.hashnode.dev/deep-dive-into-docker-unveiling-containerization-networking-and-volumes)
