# 🔒 HTTPS & Hybrid Encryption

## What is HTTPS?
HTTPS (Hypertext Transfer Protocol Secure) is HTTP layered over **TLS (Transport Layer Security)**. It runs over TCP port `443` and provides:
1. **Confidentiality:** Encrypts data against eavesdropping.
2. **Integrity:** Prevents man-in-the-middle tampering of packets.
3. **Authentication:** Proves the server's identity using digital certificates issued by trusted Certificate Authorities (CAs).

## Hybrid Encryption Model
HTTPS uses a hybrid approach to balance security and performance:
- **Asymmetric Encryption (RSA / ECC):** Used during initial handshake to securely exchange a shared session key.
- **Symmetric Encryption (AES / ChaCha20):** Used for encrypting the actual payload data with the shared session key due to its high speed.
