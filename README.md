# Running Node.js Application with Docker

This guide explains how to run a Node.js application using Docker.

## Dockerfile

To run your Node.js application using the Dockerfile:

1. **Build the Docker image**:
    ```bash
    docker build -t my-node-app .
    ```

2. **Run the Docker container**:
    ```bash
    docker run -p 3000:3000 my-node-app
    ```

This will start your Node.js application inside a Docker container. Access your application by visiting `http://localhost:3000` in your web browser.

## Docker Compose

To run your Node.js application using Docker Compose:


1. **Run Docker Compose**:

    ```bash
    docker-compose up -d
    ```

This will start your Node.js application using Docker Compose in detached mode. Access your application by visiting `http://localhost:3000` in your web browser.

## Stopping the Application

To stop the running containers:

- If you used Dockerfile:
    ```bash
    docker stop my-node-app
    ```

- If you used Docker Compose:
    ```bash
    docker-compose down
    ```

This will stop and remove the containers created by Docker or Docker Compose.
