---
tags:
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Local Area Network (LAN)]]"
---

# IP Addresses and Subnetting

## IP Addresses
All devices connected to the Internet use either a **32-bit IPv4 address** or a **128-bit IPv6 address**. Think of the IP address as a **logical address** (possibly temporary), while the **48-bit address** on every NIC is the **physical** (permanent) address.

- **[[IPv4]]**: 32-bit binary address, often written in **dotted decimal notation** for readability.
- **[[IPv6]]**: 128-bit binary address, offering a larger address space for more devices.

## IP Subnet Masking
When you have many IP addresses to manage, **subnet masking** helps break the **host ID** portion into a **subnet ID** and a **host ID**. 

**Example**: Applying a subnet mask of `255.255.255.0` to a Class B address will split the 16-bit host ID into an **8-bit subnet ID** and an **8-bit host ID**.

## Classless IP Addressing
Today, most addresses are **classless**. Instead of applying for a specific class of IP addresses, companies lease blocks of IP addresses from ISPs. This leads to more efficient allocation of addresses.

**Example**: Instead of applying for two Class C addresses, a company may lease **500 IP addresses** from an ISP, as a **contiguous block of addresses**.

## Subnetting
**Subnetting** allows a network to be divided into smaller **subnets**. 

**Need for Subnetting**:
- Classes A and B allow a large number of hosts per network, but it may be necessary to subdivide networks for **better management** and **efficiency**.

**Principle**: Use parts of the host IDs for creating **subnets**. A **subnet mask** facilitates traffic between subnets and the external network.

**Example**:
- **Subnet mask**: `255.255.255.0`
- **Address**: `192.168.1.0`
- Breaks the network into subnets with smaller broadcast domains.

## Slash Notation (CIDR)
In **slash notation**, the number after the slash represents the number of bits allocated to the **network ID**.

**Example**: 
- IP address: `167.199.170.82/27`
- This means **27 bits** are for the network ID and **5 bits** are for the host ID.
- **Subnet mask**: `255.255.255.224` (in binary: `11111111.11111111.11111111.11100000`)
- The network contains **32 addresses**.

### First and Last Address:
- **First Address**: AND the IP address with the subnet mask.
  - IP: `10100111 11000111 10101010 01010010`
  - Mask: `11111111 11111111 11111111 11100000`
  - Result: `167.199.170.64/27` (network address)
  
- **Last Address**: 31 addresses after the first.
  - Last address: `167.199.170.95/27` (broadcast address).


