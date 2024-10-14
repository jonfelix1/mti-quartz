---
tags:
  - note
  - inti
  - communcation-media-interface
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Computer Interface]]"
---

# Asynchronous Connections

**Asynchronous connections** are a method of communication at the data link layer where data is transmitted character by character in small frames.

- **Frame**: Each character is encapsulated in a small frame.
- **Start and Stop Bits**: A **start bit** is added to the front of the frame and a **stop bit** to the end to indicate the beginning and end of transmission.
- **Parity Bit** (optional): Used for **error detection**.
  
Despite the term *asynchronous*, synchronization is maintained using **start bits**. This makes it efficient for small, irregular data transfers, but **inefficient for large data transfers** due to the extra bits added to each character.
