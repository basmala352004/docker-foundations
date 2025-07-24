# Raw `docker info` Output 

---

## Client

**Version:** 28.0.4  
**Context:** desktop-linux  
**Debug Mode:** false

### Plugins

- **ai:** Docker AI Agent – Ask Gordon (v1.1.3)  
  `Path: C:\Program Files\Docker\cli-plugins\docker-ai.exe`
- **buildx:** Docker Buildx (v0.22.0-desktop.1)  
  `Path: C:\Program Files\Docker\cli-plugins\docker-buildx.exe`
- **cloud:** Docker Cloud (v0.2.20)  
  `Path: C:\Program Files\Docker\cli-plugins\docker-cloud.exe`
- **compose:** Docker Compose (v2.34.0-desktop.1)  
  `Path: C:\Program Files\Docker\cli-plugins\docker-compose.exe`
- **debug:** Get a shell into any image or container (v0.0.38)  
  `Path: C:\Program Files\Docker\cli-plugins\docker-debug.exe`
- **desktop:** Docker Desktop commands (Beta) (v0.1.6)  
  `Path: C:\Program Files\Docker\cli-plugins\docker-desktop.exe`
- **dev:** Docker Dev Environments (v0.1.2)  
  `Path: C:\Program Files\Docker\cli-plugins\docker-dev.exe`
- **extension:** Manages Docker extensions (v0.2.27)  
  `Path: C:\Program Files\Docker\cli-plugins\docker-extension.exe`
- **init:** Creates Docker-related starter files (v1.4.0)  
  `Path: C:\Program Files\Docker\cli-plugins\docker-init.exe`
- **sbom:** SBOM for an image (Anchore Inc. v0.6.0)  
  `Path: C:\Program Files\Docker\cli-plugins\docker-sbom.exe`
- **scout:** Docker Scout (v1.17.0)  
  `Path: C:\Program Files\Docker\cli-plugins\docker-scout.exe`

---

## Server

### Containers

- **Total:** 8
    - Running: 3
    - Paused: 0
    - Stopped: 5

### Images

- **Total:** 9

### Versions

- **Server Version:** 28.0.4
- **Storage Driver:** overlayfs
    - Driver Type: io.containerd.snapshotter.v1
- **Logging Driver:** json-file
- **Cgroup Driver:** cgroupfs
    - Cgroup Version: 1

### Plugins

- **Volume:** local
- **Network:** bridge, host, ipvlan, macvlan, null, overlay
- **Log Drivers:** awslogs, fluentd, gcplogs, gelf, journald, json-file, local, splunk, syslog

### CDI Spec Directories

- `/etc/cdi`
- `/var/run/cdi`

---

## Security

- **Swarm Mode:** inactive
- **Runtimes:** io.containerd.runc.v2, nvidia, runc
- **Default Runtime:** runc
- **Init Binary:** docker-init
- **containerd version:** 753481ec61c7c8955a23d6ff7bc8e4daed455734
- **runc version:** v1.2.5-0-g59923ef
- **init version:** de40ad0
- **Security Options:**
    - seccomp
        - Profile: unconfined

---

## System Details

- **Kernel Version:** 5.15.167.4-microsoft-standard-WSL2
- **Operating System:** Docker Desktop
- **OSType:** linux
- **Architecture:** x86_64
- **CPUs:** 4
- **Total Memory:** 3.747 GiB
- **Host Name:** docker-desktop
- **Docker ID:** 0e18bcea-81aa-4688-8ef8-85f919d28099
- **Docker Root Dir:** /var/lib/docker
- **Debug Mode:** false

---

## Network & Proxy

- **HTTP Proxy:** http.docker.internal:3128
- **HTTPS Proxy:** http.docker.internal:3128
- **No Proxy:** hubproxy.docker.internal

### Labels

- `com.docker.desktop.address=npipe://\\.\pipe\docker_cli`

### Experimental Features

- **Enabled:** false
- **Insecure Registries:**
    - hubproxy.docker.internal:5555
    - ::1/128
    - 127.0.0.0/8
- **Live Restore Enabled:** false
