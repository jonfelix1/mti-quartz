---
tags:
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Local Area Network (LAN)]]"
---

# Medium Access Control Protocols

## Overview

- **Medium Access Control (MAC) Protocols** determine how a workstation gains access to the **LAN medium** for data transmission.
- These protocols ensure that workstations can **"take turns"** in sending data, preventing collisions and managing network traffic.

## Categories of MAC Protocols

### [[Contention-Based Protocols]] (Statistical)

- **[[Contention-Based Protocols]]** allow multiple workstations to compete for access to the medium.
- **Statistical** in nature, these protocols use random access methods to decide which workstation gets to transmit data at a given time.
- Examples include **Carrier Sense Multiple Access with Collision Detection (CSMA/CD)** used in Ethernet.

### [[Round-Robin Protocol]] (Deterministic)

- **[[Round-Robin Protocol]]** provide a **deterministic** method for accessing the medium.
- Workstations are given a fixed time slot or order in which they can transmit data, ensuring that each workstation gets a turn.
- This method helps in managing network traffic in a more predictable manner compared to contention-based protocols.


