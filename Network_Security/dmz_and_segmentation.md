# 🏰 DMZ (Demilitarized Zone) & Network Segmentation

## What is a DMZ?
A DMZ is a physical or logical subnetwork that contains and exposes an organization's external-facing services (e.g., Web servers, Mail servers, DNS) to an untrusted network (such as the Internet), while isolating the rest of the internal corporate network.

```text
[ Internet ]
     │
[ External Firewall ]
     │
[ DMZ: Web / DNS Servers ]
     │
[ Internal Firewall ]
     │
[ Internal Private Network: Databases, HR, Finance ]
```

## Benefits:
- If a public-facing web server in the DMZ is compromised, the attacker is still blocked from directly accessing internal database systems.
