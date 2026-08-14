# 🤝 TCP Three-Way Handshake

Before TCP can transmit data reliably, it establishes a virtual connection using a **3-way handshake**.

```text
Client                                  Server
  |                                       |
  | -------- 1. SYN (seq=x) ------------> | [Server receives SYN]
  |                                       |
  | <------- 2. SYN-ACK (seq=y, ack=x+1) -| [Client receives SYN-ACK]
  |                                       |
  | -------- 3. ACK (ack=y+1) ----------> | [Connection ESTABLISHED]
```

## Step Breakdown:
1. **SYN (Synchronize):** Client chooses an initial sequence number `x` and sends a `SYN` packet to the server to initiate connection.
2. **SYN-ACK (Synchronize-Acknowledge):** Server acknowledges client sequence number with `ack = x + 1` and sends its own sequence number `y`.
3. **ACK (Acknowledge):** Client acknowledges server sequence number with `ack = y + 1`. The connection is now established and data transfer begins.
