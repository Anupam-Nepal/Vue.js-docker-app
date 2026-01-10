# Vue.js Default Application Deployed using Docker.

GitHub Repository:
https://github.com/Anupam-Nepal/Vue.js-docker-app

This repository contains a Vue.js frontend application deployed inside a Docker container.

---
## 🛠 Prerequisites

### 1. Install Docker

```bash
sudo apt update
sudo apt install -y docker.io
sudo systemctl start docker
sudo systemctl enable docker
```
### 2. Verify Installation

```bash
docker --version
```
---
### Quick Setup
#### Run these commands to install and run these applications
```bash
git clone https://github.com/Anupam-Nepal/Vue.js-docker-app.git
cd Vue.js-docker-app
docker build -t vue-app .
docker run -p 8080:80 vue-app
```
### Brief Explanation
#### 1. Clone the repository
```bash
git clone https://github.com/Anupam-Nepal/Vue.js-docker-app.git
```
Used for downloading the Vue.js Application from Github to local machine.
#### 2. Navigate to the project directory
```bash
cd Vue.js-docker-app
```
For future commands to be implemented the user must navigate to the Root directory of the project.
#### 3. Build the docker image
```bash
docker build -t vue-app .
```
Builds a Custom Docker Image named vue-app using Dockerfile.
#### 4. Run docker container
```bash
docker run -p 8080:80 vue-app
```
Runs container of the Docker Image and also maps the port 80 of container to port 8080 of the local machine.
#### 5. Access the application in browser
#### http://localhost:8080
#### Used for accessing the application.
---
### Stopping the Application
```bash
docker ps
docker stop <container_id>
```
---
### Things I Learned
1. Practical implementation of docker image and container.
2. Setting up Vue.js Environment.
3. Building custom docker image and running in it a desired port.
4. Revision of basic docker commands for running, listing and stopping containers.
---
### Difficulties I Encountered
1. Docker build failures due to incorrect Dockerfile paths.
2. Port Conflict (Already running containers exposed to same port).
