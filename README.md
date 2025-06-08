# Docker Commands
---
### Docker Desktop
A GUI for managing images and containers.

### Docker Hub
A repository to download official, verified, or sponsored images.

### Docker Engine
Responsible for creating and running containers.

### Images
Blueprints for software.

### Containers
Running instances of images.

### Volumes
External storage attached to containers.

### Network
The network component that allows containers to communicate with each other.

### Daemon
A background process also called `dockerd`.

---
### General Commands

1.  `docker login` - Log in to your Docker account.
2.  `docker logout` - Log out from your Docker account.
3.  `docker info` - Get system-wide Docker information.
4.  `docker version` - Show the Docker version.
5.  `docker help` - Get a list of all Docker commands.

---
## Image and Container Management
---
1.  `docker search <image-name>` - Search for a Docker image in Docker Hub.

2.  `docker pull <image-name>` - Get the image locally.

3.  `docker images` - View all local images.

4.  `docker create <image-name>` - Create a new container from an image.

5.  `docker ps` - List running containers.

6.  `docker ps -a` - List all containers, including exited ones.

7.  `docker run <image-name>` - Create and run a new container from an image.

8.  `docker run -it <container-name>` - Run a container in interactive mode. (Note: It's more common to use `docker run -it <image-name> <command>` to run an interactive shell inside a container, but `docker run -it <container-name>` can be used if the container has a default command to run interactively).

9.  `docker run -p <host-port>:<container-port> <image-name>` - Run an image in a container where `<container-port>` of the container is exposed at `<host-port>` on the local device.

10. `docker commit <container-name> <username>/<new-image-name>:<tag>` - Create a new custom image from a container with a custom name and tag.

11. `docker cp <file-location> <container-name>:<container-path>` - Copy a file from the local file system to a specified path within a container.

12. `docker exec <container-name> <command>` - Execute a command inside a running container.

13. `docker start <container-id>` - Start an exited container.

14. `docker stop <container-id>` - Stop a running container.

15. `docker pause <container-id>` - Pause a running container.

16. `docker rm <container-id>` - Remove a container.

17. `docker rmi <image-name>` - Remove an image.