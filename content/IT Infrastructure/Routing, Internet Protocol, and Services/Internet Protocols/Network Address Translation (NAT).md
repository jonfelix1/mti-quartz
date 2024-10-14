---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Network Address Translation (NAT)
- **NAT** allows a router to represent an entire local area network (LAN) to the Internet as a single IP address.
- **Security Feature**: By hiding the internal IP addresses of devices on a LAN, NAT adds a layer of security, making it more difficult for external entities to access internal devices.
- **Private IP Address Ranges**: NAT enables the use of private IP address ranges for internal networks, including:
  - **10.0.0.0 – 10.255.255.255**
  - **172.16.0.0 – 172.31.255.255**
  - **192.168.0.0 – 192.168.255.255**
- **Functionality**: When a device on the LAN sends a packet to the Internet, NAT changes the source IP address to the global IP address assigned to the router. The mapping of internal to external addresses is maintained in a NAT table for routing responses back to the appropriate internal device.
