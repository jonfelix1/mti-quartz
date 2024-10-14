---
tags:
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Local Area Network (LAN)]]"
---

# IPv6

## Overview
IPv6 is the **128-bit** version of the Internet Protocol (IP), designed to address the limitations of **IPv4** by providing a much larger address space. It is the latest version of the IP addressing scheme used to identify devices on a network and facilitate communication across the internet.

### Key Features of IPv6:
- **Address Length**: 128-bit address (compared to IPv4's 32-bit address).
- **Address Notation**: Uses **colon-hexadecimal notation** (e.g., `2001:0db8:85a3:0000:0000:8a2e:0370:7334`).
- **Massive Address Space**: Supports **340 undecillion** addresses, enough to meet future demands.
- **Simplified Header**: More efficient processing by routers due to a streamlined header format.
- **No Broadcasts**: IPv6 eliminates the concept of **broadcasting** and instead uses **multicast** and **anycast**.
- **Built-in Security**: IPv6 has **IPSec** (IP Security) built into the protocol, offering better data confidentiality, integrity, and authentication.

## Structure of IPv6 Address:
An IPv6 address is divided into **eight groups** of **16-bit** hexadecimal blocks, separated by colons. Each group contains **four hexadecimal digits**.

Example:
`2001:0db8:85a3:0000:0000:8a2e:0370:7334`

- **Leading zeros** in each block can be omitted.
- **Double colons** (`::`) can be used to represent consecutive blocks of zeros (only once per address).
  - **Example**: `2001:0db8::8a2e:0370:7334` is equivalent to `2001:0db8:0000:0000:0000:8a2e:0370:7334`.

## Types of IPv6 Addresses:
1. **Unicast**: Represents a single interface.
   - **Global Unicast**: Routable on the internet.
   - **Link-Local**: Only valid within the local network (`fe80::/10`).
   
2. **Multicast**: Delivers packets to multiple interfaces (replaces broadcasting).
   
3. **Anycast**: Sent to the nearest of multiple possible destinations.

## Benefits of IPv6:
- **Virtually Unlimited Addresses**: Solves the IPv4 address exhaustion issue.
- **Improved Routing Efficiency**: Simplified packet headers and hierarchical addressing reduce routing table sizes.
- **Better Multicast Support**: Enhances the delivery of multimedia content.
- **Native Support for Mobile IP**: Optimizes mobility features, especially for mobile networks.

## Transition from IPv4 to IPv6:
Since IPv4 and IPv6 are not directly compatible, **transition mechanisms** are required:
- **Dual Stack**: Devices run both IPv4 and IPv6 simultaneously.
- **Tunneling**: IPv6 packets are encapsulated within IPv4 packets for transport across IPv4 networks.
- **Translation**: Converts IPv4 to IPv6 addresses and vice versa when needed.

IPv6 adoption is crucial as the global demand for internet-connected devices continues to grow.


