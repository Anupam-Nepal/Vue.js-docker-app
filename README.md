# Laravel Application with Nginx & MySQL (Docker Compose)

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
### Running the Application
#### 1. Clone the repository
```bash
git clone https://github.com/Anupam-Nepal/Vue.js-docker-app.git
```
#### 2. Navigate to the project directory
```bash
cd Vue.js-docker-app
```
#### 3. Build the docker image
```bash
docker build -t vue-app .
```
#### 4. Run docker container
```bash
docker run -p 8080:80 vue-app
```
#### 5. Access the application in browser
#### http://localhost:8080
---
### Combined Code For Running The Application
```bash
git clone https://github.com/Anupam-Nepal/Vue.js-docker-app.git
cd Vue.js-docker-app
docker build -t vue-app .
docker run -p 8080:80 vue-app
```

### Stopping the Application
```bash
docker ps
docker stop <container_id>
```

