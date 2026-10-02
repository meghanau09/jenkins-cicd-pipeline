# Jenkins CI/CD Pipeline with Docker

## Objective

The objective of this project is to automate the build and deployment process of a Node.js application using Jenkins and Docker.

## Tools Used

- Jenkins
- Docker
- GitHub
- Node.js
- Git

## CI/CD Pipeline Flow

Developer pushes code to GitHub

↓

Jenkins Pipeline Trigger

↓

Checkout Source Code

↓

Build Docker Image

↓

Deploy Docker Container

↓

Application Running on Port 3000


## Jenkins Pipeline Stages

1. Checkout Code
   - Jenkins fetches source code from GitHub repository.

2. Build Docker Image
   - Jenkins creates a Docker image using Dockerfile.

3. Deploy Container
   - Jenkins runs the Docker container and exposes the application on port 3000.


## Docker Commands Used

Build Image:

```bash
docker build -t sample-node-app .

## Run Container:

docker run -d -p 3000:3000 --name sample-node-container sample-node-app

## Application Access

http://localhost:3000


