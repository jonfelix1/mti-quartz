---
tags:
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Local Area Network (LAN)]]"
---

# LAN Topology

## The First Local Area Network – The **Bus/Tree**


- **Original topology** for LANs
- Each **workstation** has a **Network Interface Card (NIC)** that attaches to the **bus** (a coaxial cable) through a **tap**
- **Data transfer** can occur using [[Signal]]:
  - **Baseband digital signals**
  - **Broadband analog signals**

> Bus/Tree
> ![[Pasted image 20240919203639.png#invert_B]]


## A more modern approach - The [[Star-Wired Bus]]
The [[Star-Wired Bus]] is a **network topology** that operates **logically as a bus** but is arranged **physically like a star**. Workstations are connected to a **central hub** using [[Twisted Pair Wire]]. The hub broadcasts incoming signals to all devices, making it a **shared network**. Although **installation and maintenance** are easier with modular connectors, its major drawback is that when one device transmits, **all devices hear it**, leading to potential collisions. 


A modern star wired bus use [[Switch]] instead of **Hub**

