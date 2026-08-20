# 🛡️ VPN Fundamentals (Virtual Private Networks)

## What is a VPN?
A Virtual Private Network creates a secure, encrypted tunnel over an untrusted public network (like the Internet) to connect remote users, branch offices, or cloud VPCs securely.

## How VPN Works:
1. **Encapsulation:** The original IP packet is wrapped inside a new IP packet with a new header (Tunnel mode).
2. **Encryption:** The payload data and inner headers are encrypted using strong ciphers (e.g., AES-256).
3. **Authentication:** Ensures both endpoints verify each other's identity before establishing the session.

## Split Tunneling vs Full Tunneling
- **Full Tunneling:** All internet and intranet traffic is routed through the VPN tunnel (maximum security, higher bandwidth load).
- **Split Tunneling:** Only traffic destined for corporate IP ranges goes through the VPN; normal browsing goes directly to the ISP.
