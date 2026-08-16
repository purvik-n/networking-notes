# 🤝 TLS 1.3 Handshake Flow

TLS 1.3 simplifies and speeds up the handshake to a **1-RTT (Round Trip Time)** exchange compared to 2-RTT in TLS 1.2:

```text
Client                                             Server
  |                                                  |
  | --- ClientHello + Key Share + Cipher Suites ---> |
  |                                                  |
  | <--- ServerHello + Key Share + Certificate + --- |
  |      EncryptedExtensions + Finished              |
  |                                                  |
  | --- Finished + Encrypted HTTP Application Data ->|
  |                                                  |
  | <--- Encrypted HTTP Application Response ------- |
```

### Key Improvements in TLS 1.3:
- Dropped insecure cryptographic algorithms (RC4, MD5, SHA-1, CBC mode).
- Mandatory **Forward Secrecy** via Diffie-Hellman ephemeral key exchanges.
- Zero Round Trip Time (0-RTT) resumption for returning clients.
