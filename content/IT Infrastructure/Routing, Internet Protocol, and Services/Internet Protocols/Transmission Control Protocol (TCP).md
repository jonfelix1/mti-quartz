---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Transmission Control Protocol (TCP)
- The **TCP layer** is responsible for establishing a reliable connection between a sender and a receiver using **port numbers**.
  - Each port number identifies a specific application on a device, which is associated with its **IP address**.
- TCP is capable of **multiplexing**, allowing multiple connections to coexist over a single IP line, making efficient use of network resources.

## Features of TCP
- **End-to-End Flow Control**: TCP uses a mechanism called **flow control** to ensure that the sender does not overwhelm the receiver with too much data at once. This is managed through the **Window field**, which specifies the amount of data that can be sent before requiring an acknowledgment.
- **Error Correction**: TCP employs a **Checksum** to detect errors in the transmitted data. If an error is found, the corrupted packet is retransmitted.
- **Priority Data Transmission**: TCP allows for high-priority data transmission using the **Urgent Pointer** field. This pointer indicates that certain data should be prioritized over others, ensuring timely delivery of critical information.
