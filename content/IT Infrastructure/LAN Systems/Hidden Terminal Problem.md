---
tags:
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Local Area Network (LAN)]]"
---

# Hidden Terminal Problem

## Overview

- **Hidden Terminal Problem** occurs in wireless networks when two devices cannot hear each other's transmissions but can hear a common third device.
- This situation leads to potential collisions when both devices attempt to communicate with the third device simultaneously, unaware of each other's presence.

## Example Scenario

- **Devices A and C** are within range of **Device B** but not each other.
- **Device A** and **Device C** might both attempt to send data to **Device B** at the same time, causing a collision at **Device B**.

## Solution: RTS/CTS Mechanism

> RTS/CTS
> ![[Pasted image 20240919212230.png#invert_B]]

### Request to Send (RTS) / Clear to Send (CTS)

- **RTS/CTS** is a protocol used to address the hidden terminal problem.
- It involves a two-step handshake to manage access to the shared medium and reduce the risk of collisions.

### How It Works

1. **Request to Send (RTS)**:
   - When a device wants to transmit data, it first sends an RTS frame to the intended recipient.
   - The RTS frame includes information about the duration of the transmission.

2. **Clear to Send (CTS)**:
   - The recipient of the RTS frame responds with a CTS frame if the medium is clear.
   - The CTS frame notifies all other devices in the range of the recipient that the channel is reserved for the transmission.

3. **Transmission**:
   - Once the RTS/CTS exchange is complete, the sender transmits its data.

4. **Network Awareness**:
   - Other devices that receive the CTS frame will defer their transmissions to avoid collisions.

### Benefits

- **Collision Avoidance**: Helps prevent collisions by ensuring that all devices are aware of ongoing transmissions.
- **Efficient Use of Medium**: Improves overall network efficiency by managing access to the shared medium.

### Summary

- The **Hidden Terminal Problem** can cause collisions in wireless networks when devices cannot detect each other’s transmissions.
- The **RTS/CTS Mechanism** is a solution that helps manage access to the medium and prevent such collisions through a handshake process.


