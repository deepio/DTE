# DTE
docker-tutorial-example


## Key points to remember
### Information
- `docker ps` See the status of all running containers/services
- `docker inspect <container_id>` See more detailed information about a specific container, best used with `grep`
### Control
All `docker-compose` commands affect all containers specified in the `docker-compose.yml`.
- `docker-compose up` Bring up all services
- `docker-compose exec <service_name> <command>` Executes a command in the given service
  - For example `docker-compose exec simssa bash`
- `docker-compose stop` Stops all services
- `docker-compose build` Builds all services
### Management
- `docker image rm <image_id>` Remove individual images from your computer
  - `docker image rm c2d9f4152127`
- `docker system prune -a` Remove __All__ images, containers, networks, etc. It can be helpful to know that this exists, but it can not be reversed. Be careful!
