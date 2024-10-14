---
tags:
  - note
  - inti
  - communcation-media-interface
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Computer Interface]]"
---

# Parallel vs. Serial Data Transmission


## **Parallel Data Transmission**
- Transmits **multiple bits** of data simultaneously across a set of parallel channels.
- Typically transmits **16 to 32 bits** at a time.
- **Very fast** but is best suited for **short distances** due to signal degradation over longer distances.
- Example: The internal buses of a **processor** use parallel channels for faster data transfer within the system.

## **Serial Data Transmission**
- Sends data **one bit at a time** over a single channel or wire.
- Slower compared to parallel transmission but more suitable for **long distances** as signal degradation is less of an issue.
- When data from a **serial device** needs to be processed by the CPU, it first passes through an **interface** that **buffers** and **converts** it into parallel form for compatibility with the processor.

## Key Points:
- **Parallel**: Faster, for short distances, used internally in processors.
- **Serial**: Slower, for longer distances, needs conversion when interacting with parallel-based systems.

