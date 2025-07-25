

## Namespaces & Cgroups Overview

Linux **namespaces** and **control groups (cgroups)** are core kernel features that form the foundation of containerization. Together, they isolate processes and control resource usage, enabling secure and efficient multi-tenant environments.

---

### Linux Namespaces

**Namespaces** provide isolation by giving each process its own independent view of system resources. This makes it possible to run multiple containers or services on the same host without conflicts.

#### The Six Major Namespace Types:

| Namespace                             | Isolates                                  | Description                                                           |
| ------------------------------------- | ----------------------------------------- | --------------------------------------------------------------------- |
| **mnt** (Mount)                       | File system mount points                  | Processes see only the file systems mounted in their namespace.       |
| **pid** (Process ID)                  | Process IDs                               | Each namespace has its own PID 1, allowing separate process trees.    |
| **user**                              | User and group IDs                        | Enables different UID/GID mappings, including root inside containers. |
| **net** (Network)                     | Network interfaces & routing              | Each namespace has its own network stack: IPs, routes, ports.         |
| **ipc** (Inter-Process Communication) | Semaphores, message queues, shared memory | Prevents IPC leaks across containers.                                 |
| **uts** (UNIX Timesharing System)     | Hostname & domain name                    | Allows per-container host/domain names.                               |

Namespaces improve isolation, security, and support containerized microservices.

---

### Control Groups (cgroups v2)

**Cgroups** limit and monitor resource usage (CPU, memory, I/O) for groups of processes.

#### Key Features of Cgroups v2:

* Unified resource hierarchy
* Fine-grained control over all resource types
* Better delegation and nesting support
* Improved memory and I/O management

Cgroups v2 ensures that no container can overuse system resources or starve others.

---

### Why It Matters

Namespaces **isolate**, and cgroups **control**. Together, they:

* Enable lightweight containers
* Provide process and network isolation
* Enforce resource limits and quotas
* Lay the foundation for tools like Docker, Podman, and Kubernetes

---


