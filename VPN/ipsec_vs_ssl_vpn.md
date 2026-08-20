# 🔐 IPsec vs SSL/TLS VPNs

| Feature | IPsec VPN | SSL / TLS VPN |
| :--- | :--- | :--- |
| **OSI Layer** | Layer 3 (Network Layer) | Layer 7 (Application / Transport Layer) |
| **Primary Use Case** | Site-to-Site (Router to Router) | Remote Access (Client to Gateway) |
| **Client Software** | Dedicated IPsec client software | Standard Web Browser or lightweight client |
| **Firewall Traversal** | Can be blocked by NAT/Firewalls (ESP, UDP 500/4500) | Easily passes through firewalls (Port 443 TCP) |
| **Access Scope** | Full network-level access to the subnet | Granular per-application access control |

## Modern Protocols:
- **WireGuard:** Extremely fast, modern cryptographic protocol running over UDP.
- **OpenVPN:** Flexible open-source protocol supporting both TCP and UDP.
