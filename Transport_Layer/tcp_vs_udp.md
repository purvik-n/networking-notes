# 🚀 TCP vs UDP (Transport Layer Protocols)

The Transport Layer (OSI Layer 4) provides host-to-host communication services. The two primary protocols are TCP and UDP.

| Feature | TCP (Transmission Control Protocol) | UDP (User Datagram Protocol) |
| :--- | :--- | :--- |
| **Connection Type** | Connection-oriented (Handshake required) | Connectionless (No setup required) |
| **Reliability** | Guaranteed delivery (Retransmissions) | Best-effort delivery (Packets may drop) |
| **Ordering** | Guarantees ordered arrival of packets | Packets can arrive out of order |
| **Speed / Overhead**| Slower due to headers (20-60 bytes) & acks | Extremely fast, small header (8 bytes) |
| **Flow & Congestion**| Built-in flow & congestion control | No congestion control |
| **Use Cases** | Web browsing (HTTP/HTTPS), SSH, FTP, Email | Video streaming, VoIP, Gaming, DNS queries |
