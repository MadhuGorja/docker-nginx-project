# Docker Nginx Static Website on AWS EC2

##  Project Overview

This project demonstrates how to deploy a static website using **Docker** and **Nginx** on an **AWS EC2 Ubuntu** instance.

The website consists of multiple HTML pages styled with CSS and is served through an Nginx container.

---

##  Technologies Used

- Docker
- Nginx
- AWS EC2 (Ubuntu)
- HTML5
- CSS3
- Linux
- Git & GitHub

---

##  Project Structure

```
project1/
├── index.html
├── about.html
├── contact.html
├── style.css
├── images/
└── README.md
```

---

##  What I Implemented

- Installed Docker on an AWS EC2 Ubuntu instance.
- Pulled the official Nginx image from Docker Hub.
- Created and managed Docker containers.
- Hosted a static website using an Nginx container.
- Learned Docker port mapping.
- Learned Docker bind mounts (volume mounting).
- Served website files from the host machine to the container.
- Practiced Docker container lifecycle commands.

---

##  Docker Concepts Covered

- Docker Installation
- Docker Images
- Docker Containers
- Docker Hub
- Docker Client
- Docker Daemon
- Port Mapping
- Volume Mounting (Bind Mount)
- Container Lifecycle Management

---

##  Docker Commands Used

```bash
docker pull nginx
docker images
docker run
docker ps
docker ps -a
docker stop
docker start
docker restart
docker logs
docker exec
docker rm
docker rmi
```

---

##  Deployment Workflow

```
Browser
    │
    ▼
AWS Security Group
    │
    ▼
EC2 Ubuntu Instance
    │
    ▼
Docker Engine
    │
    ▼
Nginx Container
    │
    ▼
Static Website
```

---

##  Key Learnings

- Difference between Docker and Virtual Machines.
- Difference between Docker Images and Containers.
- Running multiple containers from a single Docker image.
- Docker networking through port mapping.
- Sharing host files with containers using bind mounts.
- Hosting static websites using Nginx inside Docker.
- Managing Docker containers using the Docker CLI.

---

##  Run the Project

Pull the Nginx image:

```bash
docker pull nginx
```

Run the container:

```bash
docker run -d --name my-nginx -p 80:80 -v $(pwd):/usr/share/nginx/html nginx
```

Open your browser:

```
http://<EC2-Public-IP>
```

---

##  Future Improvements

- Build a custom Docker image using a Dockerfile.
- Host multiple websites using different containers.
- Learn Docker Compose.
- Deploy a dynamic web application with Docker.

---

##  Author

**Madhu Gorja**

B.Tech CSE Student | Cloud & DevOps Learner

GitHub: https://github.com/MadhuGorja

LinkedIn: https://www.linkedin.com/in/madhu-gorja-29781233a/
