# 🔢 IPv4 Addressing Classes & RFC 1918 Private Ranges

## IPv4 Structure
An IPv4 address consists of **32 bits** divided into 4 octets separated by dots (e.g., `192.168.1.1`). Each octet ranges from 0 to 255

## Classful Addressing (Historical)
- **Class A:** `0.0.0.0` - `127.255.255.255` (Default Mask: `255.0.0.0` /8) - Large networks
- **Class B:** `128.0.0.0` - `191.255.255.255` (Default Mask: `255.255.0.0` /16) - Medium networks
- **Class C:** `192.0.0.0` - `223.255.255.255` (Default Mask: `255.255.255.0` /24) - Small networks
- **Class D:** `224.0.0.0` - `239.255.255.255` (Multicast)
- **Class E:** `240.0.0.0` - `255.255.255.255` (Experimental / Reserved)

## Private IP Address Ranges (RFC 1918)
Private IPs are non-routable on the public internet and used inside LANs:
- `10.0.0.0` to `10.255.255.255` (`10.0.0.0/8`)
- `172.16.0.0` to `172.31.255.255` (`172.16.0.0/12`)
- `192.168.0.0` to `192.168.255.255` (`192.168.0.0/16`)
