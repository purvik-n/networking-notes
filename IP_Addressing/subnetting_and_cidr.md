# ✂️ Subnetting & CIDR (Classless Inter-Domain Routing)

## What is Subnetting?
Subnetting is the practice of dividing a large physical IP network into smaller logical sub-networks (subnets). This improves security, reduces broadcast traffic, and conserves address space.

## Understanding CIDR Notation
CIDR replaces fixed classes by appending a slash followed by the prefix length (number of 1 bits in the subnet mask).

### Common CIDR Prefixes:
- `/24` = Subnet Mask `255.255.255.0` -> $2^{32-24} = 256$ total IPs ($254$ usable hosts)
- `/25` = Subnet Mask `255.255.255.128` -> $128$ total IPs ($126$ usable hosts)
- `/26` = Subnet Mask `255.255.255.192` -> $64$ total IPs ($62$ usable hosts)
- `/28` = Subnet Mask `255.255.255.240` -> $16$ total IPs ($14$ usable hosts)

> **Rule:** For any subnet, $2$ IP addresses are always reserved:
> 1. **Network ID:** First IP (identifies the subnet)
> 2. **Broadcast Address:** Last IP (sends packets to all hosts on the subnet)
