# Technical description

## Project overview

The goal of the current project is to provide a service which is able to help its users to upload, manage and
gain insight about their purchase receipts.

## Architecture

![Architecture Diagram](/archdrawing21.11.2020.png)

## Components

![Component Diagram](/componentdiagram.png)

Production environment is configured by docker-compose and .env file on the EC2 server. Compose files are separate
for both the frontend and backend services.

### Server

Our server is located at [https://receipt.modalstudio.com/](https://receipt.modalstudio.com/) with public IP `13.53.140.53`,
hosted on AWS EC2. Services are running as [Docker](https://www.docker.com/) containers. Server installation
and Gitlab runner configuration was done manually, see [installation guide](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/blob/development/docs/aws_server.md)
for more details.

### CI/CD

Gitlab runner is set up to run tests on every branch and trigger a deployment to production on the main branch. It uses
Docker to build and update the images, compose and .env files.

### Nginx

[Nginx](https://www.nginx.com/) reverse proxy published on port `443` provides us with a single point of entry
to access our services. Client requests to the path `/api/*` are passed on to our backend service and all other paths
serve our static frontend files. Container is running on 
[receiptanalysis/frontend](https://hub.docker.com/repository/docker/receiptanalysis/frontend) with `linuxserver/letsencrypt` 
as the base image to provide us with certificate update and SSL connection.

### OCR _*(deployed, not integrated)_

Our OCR service is a small containerized python application served by [Flask](https://palletsprojects.com/p/flask/)
framework internally on port `5000`. Its goal is to provide our backend service with text extraction features from
the image files uploaded by our users using [Tesseract](https://github.com/tesseract-ocr/), 
[Tensorflow](https://www.tensorflow.org/) and [PixelLib](https://github.com/ayoolaolafenwa/PixelLib). Container
uses `ubuntu` base image. Image [receiptanalysis/ocr](https://hub.docker.com/repository/docker/receiptanalysis/ocr).

### Frontend

Our customer facing side is built on [Vue3](https://vuejs.org/) framework with some added looks by 
[Bulma](https://bulma.io/) CSS framework. Requests to the backend are done using [axios](https://www.npmjs.com/package/axios).
Static files are packaged in and served by Nginx container.

### Backend

Our backend service is providing a variety of endpoints for managing customer receipts and purchase entries connected
to them. It is also responsible for data validation and processing before saving it to persistent storage with 
[JPA](https://spring.io/projects/spring-data-jpa). Receipt images are stored on AWS S3 _*(not yet implemented)_.
Service is built using [Spring Boot](https://spring.io/projects/spring-boot) framework and running on Java 11,
published internally on port `8080`. Container is running on image 
[receiptanalysis/backend](https://hub.docker.com/repository/docker/receiptanalysis/backend) with `openjdk:11-jre-slim`
as the base image.

### Database

We are using the latest [PostgreSQL](https://registry.hub.docker.com/_/postgres) database container as our persistent
data storage published internally on port `5432`. Our models are stored in tables `customer`, `receipt` and `entry`
with relations shown on the diagram below.

![DB Diagram](/datadiagram.png)
