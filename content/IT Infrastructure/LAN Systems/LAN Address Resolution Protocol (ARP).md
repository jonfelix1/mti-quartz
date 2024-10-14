---
tags:
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Local Area Network (LAN)]]"
---

# LAN Address Resolution Protocol (ARP)

- **ARP Table**: Each **IP node** (host or router) on a LAN has an **ARP table** that stores **IP/MAC address mappings**:
    - **<IP address; MAC address; TTL>**
    - **TTL (Time To Live)**: The time after which the address mapping is forgotten (usually 20 minutes)

### ARP Protocol in Action

- **Scenario**: Host A wants to send a **datagram** to Host B
    
    - B’s **MAC address** is not in A’s **ARP table**, so A uses ARP to find B’s **MAC address**
- **ARP Query**:
    
    - A broadcasts an **ARP query** with B’s **IP address**
    - **Destination MAC address** = **FF-FF-FF-FF-FF-FF** (broadcast address)
    - All nodes on the LAN receive the **ARP query**
    - A sends:
        - **Source MAC**: **71-65-F7-2B-08-53**
        - **Source IP**: **137.196.7.23**
        - **Target IP address**: **137.196.7.14**
- **ARP Response**:
    
    - B replies with its **MAC address**, which is then stored in A’s **ARP table**


