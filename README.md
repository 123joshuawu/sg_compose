This repository allows running the below services using docker-compose:

- sg\_data
- sg\_public
- sg\_admin

### Requirements

The only required software is Docker and Docker-Compose

### Running the Services

`docker-compose up` will start all the services.

Code changes will be picked up by the services and the application will automatically update

Currently all the ports are hardcoded to the following values:
- sg\_data: 3000
- sg\_public: 8080
- sg\_admin: 8000

Type `Ctrl+c` to stop all services

`docker-compose down` will remove all containers

### Volumes

Dependencies for node (node\_modules) and php (vendor) are persisted using named volumes

Certain scenarios may require removing the volumes

The command `docker volume ls | grep sg_compose` should list all the named volumes used by this compose
