# 🔌 Layer 1 (Physical) & Layer 2 (Data Link)

## Layer 1 — Physical Layer
- **Function:** Transmits raw unstructured bit streams over a physical transmission medium.
- **PDU:** Bits (`0`s and `1`s).
- **Components:** Ethernet cables (Cat6, Fiber Optic), Wi-Fi radio frequencies, Hubs, Repeaters, Network Interface Cards (physical transceiver).

## Layer 2 — Data Link Layer
- **Function:** Provides node-to-node data transfer across the local physical network. Handles physical addressing, error detection (CRC/FCS), and framing.
- **PDU:** Frame.
- **Addressing:** Physical MAC Address (48-bit hex, e.g., `00:1A:2B:3C:4D:5E`).
- **Devices:** Network Switches, Bridges, Wireless Access Points.
- **Sublayers:**
  - **LLC (Logical Link Control):** Flow control and multiplexing protocols.
  - **MAC (Media Access Control):** Controls how devices gain access to the shared transmission medium.
