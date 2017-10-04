# Conteneurs Docker dans l'écosystème Microsoft

## Docker 101
microsoft/nanoserver

## Docker for Windows
Wrapper around windows containers (system feature)
Can switch to linux containers (run a linux VM in HyperV)
`docker run --rm -it alpine`

## Docker build (how to build permformant images?)
- Dockerfiles, actions sequence to build an image
- FROM keyword
- scratch == empty
- `docker build`
- `docker run -rm -it --name test -p 80:80 test`
- Multi-stage build (build image/run image)
- go run image--> 5Mb?

## Docker compose
- Allow deployment of multi services application
- Configuration as Code
- docker-compose.yml
- `docker-compose build` -> incremental build

## Docker and Azure
- Azure Docker Registry (portail privé)
- Azure Container Service
-- Kebernetes
-- Mesos
-- DC/OS
- Marketplace

### Cluster docker swarm (demo)

## Future
- Mixing Linux/Windows containers on the same system with the same tool
- Running linux containers on Windows without VMs