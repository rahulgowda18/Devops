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

Snapshots:
<img width="1550" height="455" alt="Screenshot 2026-02-25 002116" src="https://github.com/user-attachments/assets/177c6abe-b033-44fa-b944-ceaf07170b44" />
<img width="1386" height="731" alt="Screenshot 2026-02-25 002129" src="https://github.com/user-attachments/assets/4709e8f1-a76e-472d-aa2a-5bef646a8df2" />
