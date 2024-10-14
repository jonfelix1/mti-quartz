---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Making Connection Efficient]]"
---

# Synchronous Time Division Multiplexing (STDM)

- The original form of **time division multiplexing**.
- The **multiplexor** accepts input from devices in a **round-robin fashion** and transmits data in a continuous pattern.
- Common examples: **T-1** and **SONET telephone systems**.

> STDM Illustration
>![[Pasted image 20240912192537.png#invert_B]]

## Handling Different Data Rates

- If a device generates data at a **faster rate**, the multiplexor must either:
    - **Sample** the faster data stream more frequently.
    - **Buffer** the faster data stream.
- If a device has nothing to transmit, the multiplexor inserts a placeholder into the stream.
  
## Native Implementation
>**Bandwidth** is allocated **equally**
![[Pasted image 20240912192724.png#invert_B]]

> May waste resource sending data for **inactive terminals**
![[Pasted image 20240912193001.png#invert_B]]

## Multiplexor
>**Bandwidth** is allocated by **multiplexor**
![[Pasted image 20240912192800.png#invert_B]]

## Synchronization

- To keep the receiver synchronized with the data stream, the transmitting multiplexor may insert alternating **1s and 0s** into the data stream.
