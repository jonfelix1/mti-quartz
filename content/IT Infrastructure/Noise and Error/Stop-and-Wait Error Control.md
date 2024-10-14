---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Noise and Error]]"
---

# Stop-and-Wait Error Control

**Stop-and-Wait** is a straightforward error control protocol where the transmitter sends one frame and waits for an acknowledgment before sending the next frame.

> Stop and Wait
> ![[Pasted image 20240912205243.png#invert_B]]

- **Process**:
    - Transmitter sends a frame.
    - Waits for acknowledgment:
        - **Positive Acknowledgment (ACK)**: Proceed to send the next frame.
        - **Negative Acknowledgment (NAK)**: Retransmit the same frame.
- **Simplicity**: This method is easy to implement but can be inefficient due to waiting times.
