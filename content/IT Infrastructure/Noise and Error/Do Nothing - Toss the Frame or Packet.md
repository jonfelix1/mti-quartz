---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Noise and Error]]"
---

# Do Nothing (Toss the Frame/Packet)

**Do Nothing** is a method where the receiver discards the erroneous frame or packet without notifying the transmitter.

- **Application**: Used in some lower-layer protocols like Frame Relay.
- **Mechanism**: If an error is detected, the frame is simply discarded.
- **Assumption**: Higher-layer protocols (e.g., TCP/IP) are expected to handle retransmission by detecting the missing or erroneous frame.
