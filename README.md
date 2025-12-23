# CloudOps Docker + Nginx Deployment Project

## Overview

This project demonstrates a **CloudOps-style deployment** of a web application using **Linux, Docker, Docker Compose, and Nginx**.

The focus of this project is **infrastructure, deployment, and operations**, not application complexity.

A simple **Simon Game (HTML, CSS, JavaScript)** is deployed in a **production-like setup** to prove real-world CloudOps skills.

---

## Architecture

```
User Browser
     |
     |  (HTTP :80)
     v
Nginx (Reverse Proxy)
     |
     |  (Internal Docker Network)
     v
Docker Containers (App Instances)
```

* **Nginx** acts as the single public entry point (port 80)
* **Application containers** run on internal ports
* Only required ports are exposed

---

## Tech Stack

* Linux (Ubuntu)
* Docker
* Docker Compose
* Nginx
* HTML, CSS, JavaScript
* Git & GitHub

---

## Project Structure

```
.
├── Dockerfile
├── docker-compose.yml
├── nginx.conf
├── index.html
├── style.css
├── script.js
└── README.md
```

---

## Key CloudOps Concepts Demonstrated

* SSH-based server management
* Non-root user operations
* Containerized application deployment
* Reverse proxy configuration using Nginx
* Internal service communication via Docker network
* Clean separation between public and internal ports

---

## Deployment Steps (High-Level)

1. Create and access Linux VM via SSH
2. Install Docker and Docker Compose
3. Clone the repository
4. Build and run containers using Docker Compose
5. Access application via VM public IP on port 80

---

## How to Run

```bash
# Clone repository
git clone <repo-url>
cd cloudops-docker-nginx-project

# Build and start services
docker-compose up -d

# Verify running containers
docker ps
```

Access the application:

```
http://<VM_IP>
```

---

## Demo Video

A short demo video showing:

* Live application access via VM IP
* Running Docker containers
* Nginx reverse proxy configuration
* GitHub repository structure

( Demo link will be added here )

---

## Resume Statement

> Deployed a containerized web application on a Linux VM using Docker and Nginx, with Nginx acting as a reverse proxy on port 80, following CloudOps best practices.

---

## Notes

* Application complexity is intentionally simple
* Project emphasis is on **deployment, networking, and operations**
* Architecture mirrors real-world cloud VM deployments (e.g., AWS EC2)

---

## Author

Laksh
