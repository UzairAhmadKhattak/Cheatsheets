# Docker Commands

## General Help
- `docker (command) --help`  
  Used to get help about a specific Docker command.

## Building and Managing Images
- `docker build -t "ordo-docker" .`  
  Builds an image. The dot specifies to find the Dockerfile in the current working directory.
- `docker image ls`  
  Lists all Docker images.
- `docker rmi (hash of image)`  
  Removes an image.

## Managing Containers
- `docker rm (hash of container)`  
  Removes a container.
- `docker run (name of docker container)`  
  Runs a Docker container.
- `docker start -i (hash of container)`  
  Starts a stopped container interactively.
- `docker stop (name of container)`  
  Stops a running container.
- `docker run -it (name of image)`  
  Runs an image in a container interactively.
- `docker run -it (name of image) sh` or `docker run -it (name of image) bash`  
  Runs an image in a container with a shell (`sh` or `bash`, depending on the OS of the image).

## Logging In and Pushing to Registry
- `docker login`  
  Logs in to a Docker registry.
- `docker push (name of image)`  
  Pushes an image to a Docker registry.

## Tagging Images
- `docker image tag (name of the current tag) (new tag)`  
  Renames or retags an image.

## Detached Mode
- `docker run -d (name of image)`  
  Runs a container in detached mode, meaning that the command line will be free for other commands.
- `docker run -d --name (name of container) (name of the image)`  
  Runs a container in detached mode with a specified name.

## Viewing Logs
- `docker logs (name of the container)`  
  Views the logs of a container.
- `docker logs -f (name of the container)`  
  Follows the logs of a container in real time (`-f` for follow).

## Executing Commands in Containers
- `docker exec -it (name of container) sh`  
  Runs commands in a container interactively.

