---
tags:
  - note
  - inti
  - communcation-media-interface
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Computer Interface]]"
---


# Isochronous Connections

**Isochronous connections** are designed to handle **real-time applications** where data must be delivered at a precise rate. This type of connection is crucial in situations where timing is critical.

- **Real-time delivery**: Data must arrive **"just in time"**, meaning not too fast to overwhelm the receiver, and not too slow to cause delays in the real-time application.
- **Resource allocation**: To maintain this real-time flow, resources such as bandwidth and buffer memory are allocated at both the **sender** and **receiver** ends.

**Examples**:
- **USB** (Universal Serial Bus) and **Firewire** both support isochronous data transmission. These interfaces allow for the consistent and timely delivery of data, making them suitable for tasks like streaming video or audio, where delays or interruptions are unacceptable.

## Key Characteristics:
- **Fixed timing**: Data is transmitted at fixed intervals to maintain the flow.
- **No retransmission**: Isochronous connections do not provide mechanisms for **retransmission** of lost data because the priority is on maintaining the timing rather than perfect accuracy.
  