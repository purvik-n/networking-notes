# 🐳 Docker Network Drivers

Docker provides pluggable network drivers to control container communication:

## 1. `bridge` (Default)
Creates an isolated software bridge (`docker0`) on the host. Containers connected to the same bridge network can communicate using IP addresses or container names (on custom user-defined bridges).

## 2. `host`
Removes network isolation between container and host. The container shares the host’s networking namespace directly (highest performance, no port mapping needed).

## 3. `overlay`
Enables multi-host networking across different Docker Swarm nodes or Kubernetes clusters.

## 4. `macvlan`
Assigns a MAC address to a container, making it appear as a physical device on the LAN.

## 5. `none`
Disables all networking for the container (only localhost loopback interface available).
