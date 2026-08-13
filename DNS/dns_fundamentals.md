# 🌐 DNS Fundamentals (Domain Name System)

## What is DNS?
The Domain Name System (DNS) is often described as the **"phonebook of the Internet"**. Computers communicate using numerical IP addresses (such as `192.0.2.1` or `2600::`), while humans prefer human-readable domain names like `example.com`. DNS automatically translates domain names into IP addresses.

## DNS Hierarchy
DNS operates as a globally distributed, hierarchical tree:
1. **Root DNS Servers (`.`):** The top level of the hierarchy, directing queries to appropriate TLD servers.
2. **Top-Level Domain (TLD) Servers:** Manage extensions like `.com`, `.org`, `.net`, `.edu`, and country codes (`.in`, `.uk`).
3. **Authoritative Name Servers:** The final source of truth that holds the actual DNS records for a specific domain.

> **Key Takeaway:** Without DNS, users would need to memorize numerical IP addresses for every website and service they access.
