# Node.js Application CI/CD Pipeline Using GitHub Actions and Docker

## Project Overview

This project demonstrates an automated CI/CD pipeline for a Node.js application using GitHub Actions and Docker.

Whenever code is pushed to the main branch:
- GitHub Actions automatically triggers the workflow
- Dependencies are installed
- Application is tested
- Docker image is built
- Docker image is pushed to Docker Hub

This helps automate the software delivery process and ensures consistent deployments.

---

# Architecture / Workflow

Developer
   |
   |
GitHub Repository
   |
   |
GitHub Actions Workflow
   |
   |
Build Node.js Application
   |
   |
Create Docker Image
   |
   |
Push Image to Docker Hub


---

# Technologies Used

| Tool | Purpose |
|------|---------|
| Node.js | Application runtime |
| Docker | Containerization |
| GitHub | Source code repository |
| GitHub Actions | CI/CD automation |
| Docker Hub | Docker image registry |


---

# Project Structure
sample-node-app/
│
├── .github/
│ └── workflows/
│ └── node-ci-cd.yml
│
├── node_modules/
│
├── package.json
├── package-lock.json
├── Dockerfile
├── .dockerignore
├── .gitignore
└── README.md
