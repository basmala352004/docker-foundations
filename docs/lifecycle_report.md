
# 🐳 Docker Container Lifecycle & Disk Cleanup

This guide demonstrates the full lifecycle of a Docker container from **creation** to **removal** and how to clean up unused Docker resources using `docker image prune`. It also shows how to monitor disk usage **before and after** cleanup using `docker system df`.


## 🔁 Lifecycle Workflow

### 1. Create a container from the `nginx` image

```bash
docker create --name my-nginx nginx
```

This command creates a container named `my-nginx` from the `nginx` image 

### 2. Start the container

```bash
docker start my-nginx
```

### 3. Check disk usage before cleanup

```bash
docker system df
```

**Output:**
```
TYPE            TOTAL     ACTIVE    SIZE      RECLAIMABLE
Images          4         4         1.865GB   74.81MB (4%)
Containers      4         2         2.304MB   2.302MB (99%)
Local Volumes   7         2         1.473GB   439.1MB (29%)
Build Cache     8         0         342B      342B
```

### 4. Stop the container

```bash
docker stop my-nginx
```

### 5. Remove the container

```bash
docker rm my-nginx
```

### 6. Prune unused Docker images

```bash
docker image prune -a
```
 `-a` removes **all unused images**, not just dangling ones.


### 7. Check disk usage after cleanup

```bash
docker system df
```

**Output:**
```
TYPE            TOTAL     ACTIVE    SIZE      RECLAIMABLE
Images          3         3         1.747GB   0B (0%)
Containers      3         1         2.303MB   2.302MB (99%)
Local Volumes   7         2         1.473GB   439.1MB (29%)
Build Cache     8         0         342B      342B
```

---

## Summary of Changes

| Resource       | Before Cleanup | After Cleanup |
|----------------|----------------|----------------|
| Docker Images  | 1.865GB         | 1.747GB         |
| Reclaimable Space | 74.81MB      | 0B              |

- The `nginx` image was removed.
- The container `my-nginx` was deleted.
- Space was reclaimed using `docker image prune -a`.

---
