---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Noise and Error]]"
---

# Sliding Window Error Control

**Sliding Window** allows multiple frames to be transmitted before requiring an acknowledgment.

> Sliding Window
> ![[Pasted image 20240912205208.png#invert_B]]

- **Mechanism**:
    - **Window Size**: Defines how many frames can be sent before receiving acknowledgments.
    - **Acknowledgment**: Contains the number of the next expected frame.
- **Usage**: Commonly used in protocols like TCP with more sophisticated controls for handling multiple frames and improving efficiency.
