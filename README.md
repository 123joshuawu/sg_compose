This repository allows running the below services using docker-compose:

- sg\_data
- sg\_public
- sg\_admin

## Requirements

The only required software is Docker and Docker-Compose

## Running the Services

`docker-compose up` will start all the services.

Currently all the ports are hardcoded to the following values:
- sg\_data: 3000
- sg\_public: 8080
- sg\_admin: 8000

Type `Ctrl+c` to stop all services

`docker-compose down` will remove all containers

### For development

`docker-compose -f docker-compose.yaml -f docker-compose.development.yaml up` will run the development application

Code changes will be picked up by the services and the application will automatically update
