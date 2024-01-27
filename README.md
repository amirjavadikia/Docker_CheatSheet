# Docker Commands Cheat Sheet
Hi there 👋,
Here I'm going to show some of the most common commands in docker.

## DOCKER BASICS


* Check docker version
  ```
  docker --version
  ```
  or 
  ```
  docker -v
  ```

* Display system-wide information about docker
  ```
  docker info
  ```

* Download an image from Docker Hub
  ```
  docker pull <image_name>
  ```
  
* List local Docker images
  ```
  docker images 
  ```
  or
  ```
  docker image ls
  ```
  
* List running containers
  ```
  docker ps
  ```
  or
  ```
  docker container ls
  ```
  
* List all containers (including stopped ones)
  ```
  docker ps -a
  ```
  or
  ```
  docker container ls -a
  ```
  
* Create and start a new container from an image
  ```
  docker run <option> <image_name>
  ```

## CONTAINER LIFECYCLE

* Start a stopped container
  ```
  docker start <container_name/id>
  ```
  
* Stop a running container
  ```
  docker stop <container_name/id>
  ```
  
* Forcefully stop a running container
  ```
  docker kill <container_name/id>
  ```
  
* Restart a container
  ```
  docker restart <container_name/id>
  ```
  
* Remove a stopped container
  ```
  docker rm <container_name/id>
  ```

## IMAGES

* Build a Docker image from a DockerFile
  ```
  docker build -t <image_name> <path_to_DockerFile>
  ```
* Remove an image
  ```
  docker rmi <image_name>
  ```
* Remove all unused images
  ```
  docker image prune
  ```

## DOCKER COMPOSE

* Start services defined in a Docker Compose file
  ```
  docker-compose up
  ```
* Stop and remove services defined in a Docker Compose file
  ```
  docker-compose down
  ```
* List services in a Compose file and their status
  ```
  docker-compose ps
  ```
* View logs for a specific service
  ```
  docker-compose logs <service_name>
  ```
* run a command in a running service container
  ```
  docker-compose exec <service_name> <command>
  ```



## DOCKER REGISTRY

* Log in to a Docker registery
  ```
  docker login
  ```
* Push an image to a registry
  ```
  docker push <image_name>
  ```
* Pull an image from a registry
  ```
  docker pull <image_name>
  ```



## DOCKER NETWORKS

* Create a user-defined network
  ```
  docker network create <network_name>
  ```
* List networks
  ```
  docker network ls
  ```
* Connect a container to a network
  ```
  docker network connect <network_name> <container_name/id>
  ```
* Disconnect a container from a network
  ```
  docker network disconnect <network_name> <container_name/id>
  ```


## DOCKER LOGS AND DEBUGGING

* View Container Logs
  ```
  docker logs <container_name/id>
  ```
* Start an interactive shell in a running container
  ```
  docker exec -it <container_name/id> /bin/bash
  ```
* Display real-time container resource usage
  ```
  docker stats <container_name/id>
  ```

