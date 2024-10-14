---
tags:
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Local Area Network (LAN)]]"
---

# Round-Robin Protocol

## Overview

- **Round-robin protocols** are a type of **deterministic medium access control** method.
- They provide a **predictable and orderly** way for workstations to access the LAN medium.

## Key Features

- **Fixed Time Slots**: Each workstation is allocated a specific **time slot** or **turn** during which it can transmit data.
- **Predictable Access**: This ensures that each workstation has a scheduled opportunity to access the medium, reducing the chances of collisions.
- **Orderly Transmission**: Workstations follow a **cyclic order**, with each taking turns in a predefined sequence.

## Operation

- **Access Management**: The protocol **cycles** through all workstations in a fixed order, allowing each to transmit data during its assigned time slot.
- **Deterministic Timing**: Transmission times are predetermined, which helps in managing network traffic in a more **predictable manner** compared to contention-based methods.

## Advantages

- **Fairness**: Ensures that all workstations get a fair chance to transmit data without contention.
- **Efficiency**: Reduces the likelihood of collisions and delays, as each workstation's turn is clearly defined.

## Examples

- **Token Ring**: A classic example of a round-robin protocol, where a token circulates around the network, granting transmission rights to the workstation holding it.
- **Time-Division Multiple Access (TDMA)**: Used in various network and communication systems to allocate time slots for different users.


