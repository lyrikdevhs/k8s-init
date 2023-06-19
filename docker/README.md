# Docker([official website](https://docs.docker.com/get-started/overview/))
___
## Docker structure:
- Docker daemon
- Docker CLI
- Dockerfile
- Image
- Container
- Docker Registry

### Docker help commands:
- docker help
- docker ps -a -q
  - -a - state of all containers running and stopped
  - -q - ids the containers
- docker run --name long --rm -d long
  - -d - daemon state
  - --name - name of container
  - --rm - remove the container after it has been stopped
- docker rmi/rm ID_IMAGE_OR_CONTAINER
  - rm $(docker ps -a -q) - remove all containers
  - rmi $(docker images -q) - remove all images