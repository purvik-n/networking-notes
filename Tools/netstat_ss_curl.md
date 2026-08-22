# 💻 Socket Inspection & CLI Web Tools: netstat, ss, curl

## 1. `netstat` and `ss` (Socket Statistics)
Inspect active network connections, open ports, and listening sockets.

```bash
# Show listening TCP and UDP sockets with process names
ss -tulnp

# Show established connections
netstat -an | grep ESTABLISHED
```

## 2. `curl` (Client URL)
Command-line tool for transferring data using network protocols (HTTP, HTTPS, FTP, etc.).

```bash
# Perform verbose GET request showing TLS handshake and headers
curl -Iv https://example.com

# Send POST request with JSON payload
curl -X POST https://api.example.com/login \
  -H "Content-Type: application/json" \
  -d '{"user":"admin","pass":"secret"}'
```
