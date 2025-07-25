
# Docker Compose Lab: Nginx + Postgres App

## Objective
In this lab, you will learn to deploy a simple multi-container application using Docker Compose. This app consists of an Nginx frontend and a PostgreSQL backend.

---

## Prerequisites
- Docker & Docker Compose installed
- Internet connection
- Ubuntu or Linux-based system

---

## Step-by-Step Instructions
### 1. Install Docker and Docker Compose

```bash
curl - fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
```

### 2. Check version 
```bash
docker --version
docker compose version

```

### 3. Clone our repository 
```bash
git clone https://github.com/menaosman/docker-foundations.git
```

### 4. Authenticate using your github token to get access
 

### 5. Launch the Application
in your cloned folder run 

```bash
docker-compose up -d
```

### 6. Check Container Status
```bash
docker ps
```

### 7. Verify Nginx Web Server
Open your browser and go to: [http://localhost:8080](http://localhost:8080)

OR: ( http://<your-vm-ip>:8080 if using a VM)

### 8. Clean Up
```bash
docker-compose down -v
docker system prune -f
```

---

## What You Learned
- Define and manage multi-container apps using Docker Compose
- Use health checks and `depends_on`
- Use volumes and custom networks
- clean shutdown with system prune 

---
# it is supported with a screenshots in test.pdf file & the problem i faced and how to solve it if you had the same issue:) .
