# 🛠️ Network Diagnostics: ping & traceroute

## 1. `ping`
`ping` tests whether a destination host is reachable across an IP network and measures round-trip time.
- Operates using **ICMP (Internet Control Message Protocol)**:
  - Sends `ICMP Echo Request` (Type 8).
  - Receives `ICMP Echo Reply` (Type 0).

```bash
# Send 4 packets to Google DNS
ping -c 4 8.8.8.8
```

## 2. `traceroute` (or `tracert` on Windows)
Maps the route packets take to reach a destination host by recording every intermediate router (hop).
- Works by sending packets with incrementing **TTL (Time to Live)** values starting at $TTL=1$.
- When a router decrements $TTL$ to $0$, it drops the packet and sends back an `ICMP Time Exceeded` message, exposing its IP address.

```bash
traceroute example.com
```
