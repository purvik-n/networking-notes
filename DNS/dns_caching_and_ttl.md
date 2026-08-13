# ⚡ DNS Caching and Time-to-Live (TTL)

## What is DNS Caching?
DNS caching temporarily stores DNS query results closer to the client to reduce lookup latency and decrease load on upstream DNS servers.

## Where DNS Cache Lives:
1. **Browser Cache:** Modern browsers (Chrome, Firefox) cache DNS queries internally.
2. **Operating System Cache:** The OS DNS resolver service (e.g., Windows DNS Client cache, `systemd-resolved`).
3. **Recursive Resolver Cache:** Your ISP or public DNS provider (Google `8.8.8.8`, Cloudflare `1.1.1.1`).

## What is TTL (Time-to-Live)?
TTL is an integer value set in a DNS record (measured in seconds) that tells resolvers how long they are allowed to cache the record before asking the authoritative server again.
- **Short TTL (e.g., 300s / 5m):** Good for rapid migrations and disaster recovery.
- **Long TTL (e.g., 86400s / 24h):** Reduces DNS query overhead and speeds up page loads.
