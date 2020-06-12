# Product Microservice

This is a dockerized microservice for products. This service captures product basic information and stores them in a mongo database. You can also upload the image (jpg,png or jpeg) of the product.

## Setup

To build the express app without mongodb, run `docker build -t product-microservice`

To start the express app container, run `docker run -p 3000:3000 -d product-microservice`

### Using Docker Compose

Compose is a tool for defining and running multi-container Docker applications. With Compose, you use a YAML file to configure your application’s services. Then, with a single command, you create and start all the services from your configuration.

This application will have two services/containers: the express app and the mongodb instance. The services are declared in the docker-compose.yml file. We will be connecting the express app to the mongodb container

run `docker-compose build` to build the containers and `docker-compose up` to start the application

Alternatively, run `docker-compose up` to build and start the multi-container docker application

View api documentation at `http://localhost:3000/api-docs`
