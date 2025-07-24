# Annotated `docker info` Output

## General Metadata

- **Client Version:** `28.0.4`  
  Local Docker CLI version installed.

- **Server Version:** `28.0.4`  
  Matches client version — your daemon is in sync!

- **Context:** `desktop-linux`  
  Refers to Docker Desktop running on WSL2.

## Plugins Installed

These extend Docker’s capabilities. Notable ones:
- **Compose:** for multi-container apps
- **Buildx:** for advanced builds
- **Scout & AI Agent:** enable image insights and Docker’s assistant
- **Init:** helps scaffold starter Docker files

## Runtime & Drivers

- **Storage Driver:** `overlayfs`  
  Used to manage layered filesystems in containers.

- **Logging Driver:** `json-file`  
  Logs are saved in JSON format locally by default.

- **Cgroup Driver:** `cgroupfs`  
  Manages resource isolation for containers.

- **Runtimes Available:** `runc`, `nvidia`, `io.containerd.runc.v2`  
  Includes NVIDIA support if GPU acceleration is used.

## System Resources

- **CPUs:** `4`
- **Total Memory:** `3.747 GiB`  
  Memory available to Docker via WSL2.

- **Architecture:** `x86_64`
- **Operating System:** `Docker Desktop on Windows with Linux backend (WSL2)`
- **Kernel:** `5.15.167.4-microsoft-standard-WSL2`

## Security

- **Seccomp Enabled:** `Yes`
- **AppArmor:** Not shown in output (likely disabled in WSL2)
- **Profile:** `unconfined` — lowest restrictions on containers

## Proxy Configuration

- **HTTP Proxy:** `http.docker.internal:3128`
- **HTTPS Proxy:** `http.docker.internal:3128`
- **No Proxy:** for local/internal addresses

## Container Stats

- **Containers:** `8` total
    - `3` running
    - `5` stopped
- **Images:** `9` total
- **Volumes:** Not explicitly listed (but plugin `local` is present)

## Swarm

- **Swarm Mode:** Inactive  
  You’re not using Docker Swarm for orchestration.

## Observations

- **Live Restore Enabled:** `false`  
  Containers will stop when the daemon restarts — not persistent across restarts.

- **Experimental Features:** `false`  
  Default stable mode — no beta/test features enabled.

