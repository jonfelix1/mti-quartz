---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Forwarding Table Layer

## Layer 2 (Data Link Layer)

- **Switches** operate at Layer 2.
- They use **L2 [[Forwarding Table]]** to manage the forwarding of packets within a **local area network (LAN)**.
- The table is built using **dynamic learning algorithms**, where the switch learns the MAC addresses of devices.
- When the switch knows the destination address, it sends the packet only to the corresponding link/segment.
- If the destination is unknown, the switch performs **flooding**.

## Layer 3 (Network Layer)

- **Routers** operate at Layer 3.
- They use **L3 [[Forwarding Table]]** (also known as **routing tables**) to manage the forwarding of packets across networks.
- Routers use **routing protocols** (e.g., OSPF, BGP) to learn about the network and make forwarding decisions.
- Routers always forward packets based on the network layer addresses (e.g., IP addresses) and never broadcast.

## Comparison

- **L2 [[Forwarding Table]]** are used for **MAC addresses** within a local network, while **L3 [[Forwarding Table]]** handle **IP addresses** for inter-network communication.
- Switches handle communication within the same network, while routers handle communication between different networks.
