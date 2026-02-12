# Docker Learning

This repository contains my Docker practice, commands, and sample setups while learning Docker.

## About
I am learning Docker to understand how applications can be packaged and deployed using containers. This repository stores commands and practice notes for future reference and continuous learning.

## ⚙️ Docker Commands – Learning Notes

```bash
 1. Pull an Image from Docker Hub
docker pull <image_name>

2. List Downloaded Images
docker images
Shows all Docker images available locally.

3. Create and Run a Container
docker run <image_name>
Creates and runs a new container from the specified image.

4. Run Container in Interactive Mode
docker run -it <image_name>
Runs container in interactive mode so we can access the container terminal (for example, Ubuntu shell).

5. Show All Containers
docker ps -a

6. Show Running Containers Only
docker ps

7. Start an Existing Container
docker start <container_name_or_id>

8. Stop a Running Container
docker stop <container_name_or_id>

9. Remove an Image
docker rmi <image_name>

10. Remove a Container
docker rm <container_name_or_id>

11. Pull Specific Image Version
docker pull <image_name>:<version>

12. Run Container in Detached Mode
docker run -d <image_name>

13. Run Container with Custom Name
docker run -d --name <container_name> <image_name>

14. Docker Images and Layers
Docker images are built as a **collection of layers**, where each layer represents a change or instruction added to the image.  
This layered structure makes images lightweight and efficient because layers can be reused across images.

15. Port Binding in Docker
Port binding maps a **host machine port** to a **container port**, allowing services inside containers to be accessed from outside.

Command format:
```bash
docker run -p <host_port>:<container_port> <image_name>
Example:
docker run -d -e MYSQL_ROOT_PASSWORD=secret --name mysql-older -p 5000:3306 mysql:8.0
```
16. View Container Logs
```bash
docker logs <container_name_or_id>
```
17. Follow Logs in Real-Time
```
docker logs -f <container_name_or_id>
```
---



