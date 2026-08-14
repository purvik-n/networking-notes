# 🔌 TCP Connection Teardown & Control Flags

## TCP 4-Way Connection Teardown
Closing a TCP connection gracefully requires a 4-step termination process using `FIN` and `ACK` packets:

1. **Client -> Server (FIN):** Client has finished sending data and requests connection closure.
2. **Server -> Client (ACK):** Server acknowledges receipt of client's closure request.
3. **Server -> Client (FIN):** Server finishes its remaining data transmission and signals closure.
4. **Client -> Server (ACK):** Client acknowledges server's FIN, enters `TIME_WAIT` state, and closes.

## Essential TCP Control Flags:
- **SYN (Synchronize):** Initiates a connection.
- **ACK (Acknowledgment):** Confirms receipt of packets.
- **FIN (Finish):** Requests graceful connection termination.
- **RST (Reset):** Abruptly aborts a faulty or invalid connection.
- **PSH (Push):** Asks the receiver to push buffered data immediately to the application.
- **URG (Urgent):** Indicates segment contains high-priority data.
