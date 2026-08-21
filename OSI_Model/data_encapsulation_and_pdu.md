# 📦 Data Encapsulation & Protocol Data Units (PDU)

As data moves down the OSI stack during transmission, each layer prepends its own header (and trailer) to the payload. This process is called **Encapsulation**.

```text
[ Application Data ]
       ↓ (Layer 4 adds TCP/UDP Port Header)
[ TCP Header | Data ]                                  --> Segment
       ↓ (Layer 3 adds Source & Dest IP Header)
[ IP Header | TCP Header | Data ]                      --> Packet
       ↓ (Layer 2 adds MAC Header & FCS Trailer)
[ MAC Header | IP Header | TCP Header | Data | FCS ]  --> Frame
       ↓ (Layer 1 converts to physical signal)
01011010010101100010101010100101010101                 --> Bits
```

When received on the destination host, the reverse process (**De-encapsulation**) occurs as headers are parsed and stripped away layer-by-layer.
