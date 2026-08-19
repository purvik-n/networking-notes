# 🔌 Docker Port Mapping & Commands

## Port Publishing Syntax:
```bash
docker run -d -p <HOST_PORT>:<CONTAINER_PORT> --name my-web nginx
```

Example:
```bash
docker run -d -p 8080:80 nginx
```
- Traffic arriving at host port `8080` is forwarded by iptables/Docker proxy to container port `80`.

## Useful Docker Network Commands:
```bash
# List all networks
docker network ls

# Create a custom user-defined bridge
docker network create my-custom-net

# Inspect network details and connected containers
docker network inspect my-custom-net

# Connect running container to network
docker network connect my-custom-net my-container
```
