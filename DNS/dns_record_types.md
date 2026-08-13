# 📋 Common DNS Record Types

DNS databases store different types of records for various networking purposes:

| Record Type | Name | Purpose | Example |
| :--- | :--- | :--- | :--- |
| **A** | Address Record | Maps a hostname to a 32-bit IPv4 address | `example.com -> 93.184.216.34` |
| **AAAA** | IPv6 Address | Maps a hostname to a 128-bit IPv6 address | `example.com -> 2606:2800:220:1::` |
| **CNAME** | Canonical Name | Creates an alias pointing one domain name to another | `www.example.com -> example.com` |
| **MX** | Mail Exchange | Specifies mail servers responsible for receiving email | `mail.example.com (Priority: 10)` |
| **TXT** | Text Record | Carries arbitrary text, used for SPF, DKIM, verification | `v=spf1 include:_spf.google.com ~all` |
| **NS** | Name Server | Delegates a DNS zone to an authoritative server | `ns1.nameserver.com` |
| **PTR** | Pointer Record | Used for reverse DNS lookups (IP to domain name) | `34.216.184.93.in-addr.arpa` |
