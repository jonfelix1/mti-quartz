---
tags:
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Local Area Network (LAN)]]"
---

# MAC Addresses

- **32-bit IP address**:
    - **Network-layer address** for an interface
    - Used for **layer 3 (network layer) forwarding**
    - Example: **128.119.40.136**
- **MAC address** (also called LAN, physical, or Ethernet address):
    - **Function**: Used **locally** to transfer a **frame** from one interface to another within the **same subnet** (in terms of IP addressing)
    - **48-bit MAC address**:
        - Burned into **NIC ROM** (Network Interface Card Read-Only Memory)
        - Sometimes **software-settable**
    - Example: **1A-2F-BB-76-09-AD**
- **Hexadecimal (base 16) notation**:
    - Each **numeral** represents **4 bits**
- Router sends data through [[LAN Address Resolution Protocol (ARP)]]

### Interface Addresses on a LAN

- Each interface on a LAN has:
    - A unique **48-bit MAC address**
    - A **locally unique** **32-bit IP address**

### MAC Address Administration

- **MAC address allocation** is administered by **IEEE**
- Manufacturers buy a portion of **MAC address space** to ensure **uniqueness**
- **Analogy**:
    - **MAC address**: like a **Social Security Number**
    - **IP address**: like a **postal address**

### MAC Address Portability

- **MAC address flat**: Portable; can move an interface from one LAN to another
- **IP address**: Not portable; depends on the **IP subnet** to which the node is attached


