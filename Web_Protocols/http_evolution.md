# 🚀 Evolution of HTTP: HTTP/1.1 vs HTTP/2 vs HTTP/3

## HTTP/1.1 (1997)
- Text-based protocol.
- Suffered from **Head-of-Line (HoL) blocking** at the application layer.
- Required multiple parallel TCP connections to fetch assets simultaneously.

## HTTP/2 (2015)
- Binary framing layer.
- **Multiplexing:** Multiple requests and responses sent simultaneously over a single TCP connection.
- **Header Compression (HPACK):** Reduces overhead of repeated headers.
- **Server Push:** Server can push resources before client requests them.

## HTTP/3 (2022)
- Replaces TCP with **QUIC** (built on top of UDP).
- Eliminates TCP Head-of-Line blocking (packet drop on one stream doesn't stall others).
- Faster connection establishment with built-in TLS 1.3 encryption.
