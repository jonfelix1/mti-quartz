---
tags:
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Local Area Network (LAN)]]"
---

# IPv4

## Overview
IPv4 (Internet Protocol version 4) is the **fourth version** of the Internet Protocol (IP) and the most widely used to identify devices on a network and route traffic across the internet. It is based on a **32-bit address** system, allowing for around **4.3 billion unique addresses**.

### Key Features of IPv4:
- **Address Length**: **32-bit address**.
- **Address Notation**: Written in **dotted decimal notation** (e.g., `192.168.1.1`).
- **Supports Broadcast**: IPv4 allows for **broadcasting** to communicate with all devices on a local network.
- **Dynamic Addressing**: Uses **DHCP (Dynamic Host Configuration Protocol)** to dynamically assign IP addresses to devices.
- **Limited Security**: IPv4 was designed without inherent security features, although security protocols such as **IPSec** can be added.

## Structure of IPv4 Address:
An IPv4 address consists of **four octets** (or bytes), separated by periods. Each octet is represented as a **decimal number** between **0 and 255**.

Example:
`192.168.1.1`

- **Binary Representation**: Each octet in decimal is converted to an 8-bit binary number.
  - Example: `192.168.1.1` in binary is `11000000.10101000.00000001.00000001`.

## IPv4 Address Classes:
IPv4 addresses are divided into **five classes** based on their range and usage:

| **Class** | **Range** (First Octet) | **Purpose**               |
| --------- | ----------------------- | ------------------------- |
| **A**     | 0 - 127                 | Large networks            |
| **B**     | 128 - 191               | Medium-sized networks     |
| **C**     | 192 - 223               | Small networks            |
| **D**     | 224 - 239               | Multicast groups          |
| **E**     | 240 - 255               | Experimental use          |

### Private Address Ranges:
Certain IPv4 addresses are reserved for **private networks** and are not routable on the public internet:

- **10.0.0.0 – 10.255.255.255** (`10.0.0.0/8`)
- **172.16.0.0 – 172.31.255.255** (`172.16.0.0/12`)
- **192.168.0.0 – 192.168.255.255** (`192.168.0.0/16`)

## Subnetting:
**Subnetting** allows the division of a large network into smaller, manageable sub-networks (subnets). A **subnet mask** helps distinguish between the network portion and the host portion of an IP address.

- **Example**: The subnet mask `255.255.255.0` applied to an IPv4 address breaks it into **24 bits** for the network ID and **8 bits** for the host ID.

## IPv4 Limitations:
- **Limited Address Space**: Only around **4.3 billion addresses** are available, leading to **address exhaustion**.
- **No Built-in Security**: IPv4 was not designed with security features, though IPSec can be added externally.
- **Broadcasting**: Broadcasting can lead to inefficiencies and increased network traffic.

## Transition to IPv6:
Due to the **exhaustion of IPv4 addresses**, IPv6 was developed. However, IPv4 is still in widespread use, with many networks implementing **dual-stack** solutions to support both protocols during the transition.

IPv4 remains foundational to internet communication despite the move towards IPv6 for better scalability and security.


