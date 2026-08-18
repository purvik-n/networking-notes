# 🛡️ IDS vs IPS (Intrusion Detection vs Prevention)

Both IDS and IPS inspect network traffic for known attack patterns (signatures) or unusual baseline behavior (anomalies).

| Feature | IDS (Intrusion Detection System) | IPS (Intrusion Prevention System) |
| :--- | :--- | :--- |
| **Placement** | Out-of-band (Span / Tap port) | In-line (Traffic passes directly through it) |
| **Action** | Passive: Detects attacks, logs, sends alerts | Active: Drops malicious packets, resets connections |
| **Network Impact** | Zero latency impact on network traffic | Can introduce slight latency; false positives drop legitimate traffic |
| **Analogy** | A security camera with a motion alarm | An armed security guard at the gate |
