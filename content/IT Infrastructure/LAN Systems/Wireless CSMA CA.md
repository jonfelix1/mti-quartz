---
tags:
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Local Area Network (LAN)]]"
---

# Wireless CSMA/CA

> CSMA/CA Algorithm
> ![[Pasted image 20240919212035.png#invert_B]]

## Overview

- **CSMA/CA** stands for **Carrier Sense Multiple Access with Collision Avoidance**.
- Unlike **CSMA/CD** (Collision Detection), CSMA/CA does not detect collisions once they occur. Instead, it aims to **avoid collisions** before they happen.

## How CSMA/CA Works

- **Inter Frame Space (IFS)**: All devices must wait for a specific amount of time, called an **Inter Frame Space (IFS)**, before they can transmit data.
  - **Short IFS**: Used by some applications for quicker transmission.
  - **Long IFS**: Used by other applications that might need more time before transmission.

- **Collision Avoidance Mechanism**:
  - If two devices attempt to transmit at the same time, the device with the shorter IFS will go first.
  - This reduces the likelihood of collisions by prioritizing transmissions based on the IFS.

## Key Points

- **IFS Values**: Vary depending on the technology and application.
- **Collision Avoidance**: By regulating transmission timing and prioritizing based on IFS, CSMA/CA helps manage network traffic and minimize collisions in wireless networks.


