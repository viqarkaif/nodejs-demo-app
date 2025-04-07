# Automated CI/CD Pipeline for Node.js App using GitHub Actions & DockerHub

This project demonstrates a simple Node.js application integrated with a CI/CD pipeline using **GitHub Actions** and **DockerHub**.

## 🔧 Project Setup

- **GitHub Repo**: [nodejs-demo-app](https://github.com/viqarkaif/nodejs-demo-app)
- **DockerHub Repo**: [viqarkaif/nodejs-demo-app](https://hub.docker.com/r/viqarkaif/nodejs-demo-app)

## 🚀 CI/CD Workflow Overview

Every push to the `main` branch triggers the following workflow:

1. Checkout source code
2. Set up Docker Buildx
3. Log in to DockerHub using GitHub Secrets
4. Build Docker image
5. Push image to DockerHub

## 🛠 Requirements

- Node.js v18+
- Docker installed
- DockerHub credentials added to GitHub Secrets:
  - `DOCKERHUB_USERNAME`
  - `DOCKERHUB_TOKEN`

## 📁 Project Structure

```
.
├── .github/workflows/docker-image.yml
├── Dockerfile
├── package.json
└── index.js
```

## 📦 Docker Image

```bash
# Pull the latest image
docker pull viqarkaif/nodejs-demo-app:latest

# Run the container
docker run -p 3000:3000 viqarkaif/nodejs-demo-app
```

---

📝 **Project Title**: Automated CI/CD Pipeline for Node.js App using GitHub Actions & DockerHub  
© 2025 Mohd Viqar Ullah kaif | Built with ❤️
# nodejs-demo-app
