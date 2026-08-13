# 🔄 How DNS Lookup Works (Resolution Flow)

When you type `https://www.example.com` into your browser, the following lookup sequence occurs:

```text
Browser -> Local DNS Cache (OS / Router)
               ↓ (Cache Miss)
Recursive Resolver (ISP / 8.8.8.8 / 1.1.1.1)
               ↓
Root Name Server (.)
               ↓
TLD Name Server (.com)
               ↓
Authoritative Name Server (example.com)
               ↓
Returns IP to Recursive Resolver -> Browser connects to Web Server!
```

## Recursive vs Iterative Queries
- **Recursive Query:** The client asks the DNS resolver to do all the work and return the final answer or an error.
- **Iterative Query:** The resolver asks name servers, and each server responds with a referral to the next server down the hierarchy until the authoritative server is reached.
