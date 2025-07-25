Namespaces & Cgroups Overview

Linux namespaces and cgroups are two foundational features that enable containerization by isolating and managing resources per process.

Namespaces isolate system resources, allowing each process (or container) to have its own independent view of the system. This makes it possible to run multiple services on the same host without interference.

There are six major types of Linux namespaces:

Mount (mnt): Isolates the set of mounted file systems.

PID: Provides each namespace with its own process ID space. PID 1 is the first process in that namespace.

User: Allows a process to have different user and group IDs. Processes can have root privileges inside their own user namespace without having root access on the host.

Network (net): Gives a separate network stack with independent interfaces, routing tables, and firewall rules.

IPC: Isolates interprocess communication mechanisms such as message queues and semaphores.

UTS: Enables different hostnames and domain names for each namespace.

The key feature of namespaces is their ability to isolate processes from one another. This improves security, reduces the blast radius of failures, and supports microservice-based architectures.

Cgroups (Control Groups) complement namespaces by controlling and monitoring system resources. Cgroups v2, the latest version, introduces a unified hierarchy for managing all resources consistently. It offers improved delegation, simplified resource control, and more effective handling of memory and I/O.

Together, namespaces and cgroups provide the essential building blocks for Linux containers. They allow for secure, isolated, and resource-managed environments, which are critical for running modern distributed applications.