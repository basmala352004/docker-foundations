
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


## Commands of hello-world.cast file 


| CLI Flag             | Description                                                                  |
|----------------------|-------------------------------------------------------------------------------|
| `docker run`         | Starts a new container from the specified image.                             |
| `-p 49160:80`        | Maps container port 80 to host port 49160 (demo use only).                   |
| `--name hello-demo`  | Assigns a custom name to the container.                                      |
| `hello-world`        | Specifies the image to use — pulled from Docker Hub if not found locally.    |


## How to Play `.cast` Recordings

This section explains how to preview terminal recordings from `.cast` files depending on your operating system.

---

### Linux / Unix Users

To play a `hello-world.cast` file in your terminal:

asciinema play hello-world.cast


### Windows Users 

You can preview `hello-world.cast` files directly using an online web player:

**Web Player Link:** [https://latinsud.com/pub/asciinema](https://latinsud.com/pub/asciinema)

**Steps to preview:**

1. Open the link above in your browser
2. Drag and drop the `hello-world.cast` file into the page
3. The terminal recording will play automatically

---
# it is supported with a screenshots in test.pdf file & the problem i faced and how to solve it if you had the same issue:) .
