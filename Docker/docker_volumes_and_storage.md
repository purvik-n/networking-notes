# 💾 Docker Volumes & Persistent Storage

By default, container filesystems are **ephemeral**; when a container is deleted, changes to its writable layer are lost.

## Storage Types in Docker:
1. **Named Volumes (`docker volume create`):** Managed completely by Docker in `/var/lib/docker/volumes/`. Best practice for production databases.
2. **Bind Mounts (`-v /host/path:/container/path`):** Mounts a specific directory or file from the host filesystem directly into the container.
3. **`tmpfs` Mounts:** Stored only in host memory (RAM), never written to host filesystem or container writable layer.

```bash
# Run PostgreSQL with persistent volume
docker run -d \
  --name postgres-db \
  -v pgdata:/var/lib/postgresql/data \
  -e POSTGRES_PASSWORD=secret \
  postgres:alpine
```
