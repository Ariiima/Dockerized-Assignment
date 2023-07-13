# UltraFusion Assignment

This repository contains the code for the UltraFusion assignment, which consists of a React application and a server component.

## React App

The React app is located in the `my-app` directory. It is a frontend application built using React.

## Installation

First Clone the repository using:
```git clone https://github.com/Ariiima/Dockerized-Assignment.git```

Then you shold use these commands to also clone the submodules:
```git submodule init
    git submodule update```

## Docker Compose

The project is configured with Docker Compose to run multiple containers. The Docker Compose file is located in the root directory.

To build and run the project using Docker Compose, run the following command:

```docker-compose up```


This command will build the Docker images for the React app, the server, and the Redis server, and start the containers.

The React app will be accessible at `http://localhost`.

The server will be accessible at `http://localhost:3000`.

### API Endpoints

The server exposes the following API endpoints:

- `GET /prompts`: Retrieves the list of prompts.
- `GET /prompts/:id`: Retrieves a specific prompt by ID.
- `POST /prompts`: Creates a new prompt.
example:
```
{
    "title":"prompt title",
    "description":"a short description",
    "prompt":"prompt itself"
}
```
- `PUT /prompts/:id`: Updates an existing prompt.
- `DELETE /prompts/:id`: Deletes a prompt.

## Dependencies

The project has the following dependencies:

- React: A JavaScript library for building user interfaces.
- Express: A web application framework for Node.js.
- Redis: An in-memory data store used for persistence.

