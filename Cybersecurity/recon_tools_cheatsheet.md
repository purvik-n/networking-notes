# 🔍 Reconnaissance & Footprinting Cheat Sheet

## Passive Reconnaissance (No direct target interaction)
- **`whois example.com`** — Look up domain registration and ownership records.
- **`nslookup -type=any example.com`** — Query DNS records and mail servers.
- **`dig example.com +trace`** — Trace DNS lookup path.
- **`shodan.io`** — Search engine for internet-connected devices and exposed services.

## Active Reconnaissance (Direct interaction with target)
- **Nmap Port Scanning:**
  ```bash
  nmap -sS -sV -O -T4 192.168.1.1
  ```
  - `-sS`: SYN Stealth scan
  - `-sV`: Detect service and version info
  - `-O`: OS detection
  - `-T4`: Aggressive timing template
