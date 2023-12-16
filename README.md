# Docker Commands Cheat Sheet
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
