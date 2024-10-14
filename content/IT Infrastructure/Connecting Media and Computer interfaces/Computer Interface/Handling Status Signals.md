---
tags:
  - note
  - inti
  - communcation-media-interface
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Computer Interface]]"
---

# Handling Status Signals

Manages signals that indicate the status of peripheral devices.

## Duplexity

**Duplexity** refers to the direction and method of data transmission between two devices.

- **Simplex**: Data can only be transmitted in one direction. One device is always the sender, and the other is always the receiver.
- **Half-Duplex**: Data can be transmitted in both directions, but only one direction at a time. Communication alternates between sending and receiving.
- **Full-Duplex**: Data can be transmitted in both directions **simultaneously**, allowing faster and more efficient communication.


## Connections
Connection have 3 types:
- [[Asynchronous Connections]]: Transfer data in smaller frames
- [[Synchronous Connections]]: Transfer data in large frames
- [[Isochronous Connections]]: Used to handle real time application

## Synchronous vs Asynchronous Example

**Asynchronous connection** (700K chars file):
- Each character has a start bit, stop bit, and possibly a parity bit.
- **Data size**: 700,000 chars × 11 bits (8 bits data + 1 start + 1 stop + 1 parity) = **7,700,000 bits**.

**Synchronous connection** (700K chars file):
- Assumes a **maximum payload size** of 1500 bytes (1,500 characters per frame).
- Each frame contains **5 bytes of overhead** (1-byte header, 1-byte address, 1-byte control, 2-byte checksum).
- **Data size**: 
  - 1500 bytes payload + 5 bytes overhead = 1505 bytes per frame.
  - 467 frames × 1505 bytes = **716,380 bytes**, or **5,731,040 bits**.

**Conclusion**: Synchronous connections require significantly **less data** for the same file transfer compared to asynchronous connections due to the reduced overhead.
