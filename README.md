🚀 MEAN Stack DevOps Deployment
📌 Project Overview

Containerized and deployed a full-stack MEAN application using Docker, Docker Compose, GitHub Actions CI/CD, and Nginx reverse proxy.

🏗 Architecture

User → Nginx (Port 80) → Frontend → Backend → MongoDB

🐳 Docker Setup
Build Images
docker build -t username/devops_backend ./backend
docker build -t username/devops_frontend ./frontend
Run with Docker Compose
docker-compose up -d
🔁 CI/CD Pipeline

Triggered on push to main branch

Builds Docker images

Pushes to Docker Hub

SSH into VM

Pulls latest images

Restarts containers automatically

🌐 Nginx Reverse Proxy

Only port 80 exposed

Routes:

/ → Frontend

/api → Backend
