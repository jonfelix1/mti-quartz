---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Address Resolution Protocol (ARP)
- **ARP** is essential for translating IP addresses into **MAC layer addresses**. When an IP packet arrives at a local network, it needs the MAC address of the destination device to deliver the frame.
- **How It Works**: When a device wants to communicate with another on the same local area network, it broadcasts an ARP request to find the MAC address corresponding to the destination IP address. The device with the matching IP address responds with its MAC address.
- **Importance**: ARP is crucial in bridging the gap between Layer 2 (Data Link layer) and Layer 3 (Network layer) in the OSI model, enabling effective communication in local networks.