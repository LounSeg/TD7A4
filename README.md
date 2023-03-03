# TD7A4

## Prerequisites
Before proceeding with the instructions, make sure that you have installed the following:

- Docker - You can download and install Docker from https://docs.docker.com/get-docker/
- Docker-compose - You can download and install Docker-compose from https://docs.docker.com/compose/install/

## Running Containers with Docker Image
To run your own containers using Docker image, follow these steps:

1. Pull the Docker image by running the following command:

```
docker pull <docker-image-name>
```

2. Create a Docker container from the image by running the following command:

```
docker run --name <container-name> -d <docker-image-name>
```
Replace `<container-name>` with the name you want to give to your container and `<docker-image-name>` with the name of the Docker image you want to use.

3. Check if the container is running by running the following command:

```
docker ps
```
This will display a list of running containers.

## Running Containers with Docker-compose
To run your own containers using Docker-compose, follow these steps:

1. Create a Docker-compose file named `docker-compose.yml` in your project directory with the following content:

```
version: "3.9"

services:
  <service-name>:
    image: <docker-image-name>
    container_name: <container-name>
    restart: always
```
Replace <service-name> with the name you want to give to your service, `<container-name>` with the name you want to give to your container, and `<docker-image-name>` with the name of the Docker image you want to use.

2. Start the containers by running the following command:

```
docker-compose up -d
```

This will create and start the containers defined in the docker-compose.yml file in the background.

3. Check if the containers are running by running the following command:

```
docker-compose ps
```

This will display a list of running containers.



Congratulations! You have successfully created and started your own containers using Docker image and Docker-compose.
