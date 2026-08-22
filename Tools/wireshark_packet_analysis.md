# 🦈 Wireshark Packet Analysis

Wireshark is an open-source packet analyzer used for network troubleshooting, protocol analysis, and security auditing.

## Key Capture Concepts:
- **Promiscuous Mode:** Allows the network card to capture all packets traveling across the local segment, not just packets destined for its own MAC address.
- **Pcap format:** Standard packet capture file format (`.pcap`, `.pcapng`).

## Essential Display Filter Expressions:
```text
# Filter by IP address
ip.addr == 192.168.1.50

# Filter by TCP Port
tcp.port == 443

# Filter by protocol
http || dns || icmp

# Filter HTTP POST requests
http.request.method == "POST"

# Filter TCP Handshake SYN packets
tcp.flags.syn == 1 && tcp.flags.ack == 0
```
