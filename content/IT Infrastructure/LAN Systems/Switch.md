---
tags:
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Local Area Network (LAN)]]"
---

# Switch

> Switch
> ![[Pasted image 20240919205207.png#invert_B]]

- **Switches** create a unique **network segment** on each port, **separating collision domains**, improving network performance and bandwidth.
- Unlike hubs, switches can intelligently **filter and forward**  data based on the **NIC (MAC) address** of devices.
- **Switches** use **forwarding tables** to route data between computers, learning this information automatically from incoming packets.

## Key Features of Switches

- **Direct connection**: Hosts are directly connected to the switch, allowing simultaneous data transfers like A-to-A' and B-to-B' without collisions.
- **Cascading**: Switches can be cascaded to expand the network.
- **Filtering frames**: Unlike hubs, which broadcast incoming frames to all ports, switches **forward frames** to specific devices based on *[[MAC Addresses]].
  
## Switch vs. Hub

> Workstations connected to a shared segment [[Local Area Network (LAN)]]
> ![[Pasted image 20240919205252.png#invert_B]]

> Workstations connected to a dedicated segment [[Local Area Network (LAN)]]
>![[Pasted image 20240919205329.png#invert_B]]

- **Hubs**: Simply transmit incoming frames to all ports, creating a **shared network** segment.
- **Switches**: Provide **dedicated segments** for each device, eliminating **collisions** and improving performance.

## Advantages of Switches

- **Simultaneous transmissions**: Multiple devices can communicate simultaneously without collisions.
- **Efficient isolation**: Heavy users can be isolated from the rest of the network, optimizing traffic.
- **Full duplex**: Links use [[Full-Duplex Switches]] for communication, preventing collisions.

## Switch Backplane and Cut-Through Architecture

- **Backplane**: The switch's backplane is fast enough to support multiple data transfers at once.
- **Cut-through architecture**: Allows the switch to start forwarding a frame before it is fully received, reducing latency.

## Ethernet Switch

- **Link-layer device**: Switches operate at the **link layer** (layer 2) and manage the forwarding of **Ethernet frames**.
- **Transparent**: Hosts are unaware of the switch's presence.
- **Plug-and-play**: Switches are **self-learning** and do not require configuration.

## Switch Tables and Self-Learning

- **Switch table**: Keeps track of [[MAC Addresses]], the **interface** they are reachable through, and a **timestamp** (TTL).
- **Self-learning**: When a frame is received, the switch learns the sender's location and updates its table. If the destination is unknown, the switch floods the frame to all ports except the incoming one.
- **Frame filtering/forwarding**: Switches filter frames by checking their **MAC destination address** in the switch table.

## Self-Learning Example

| MAC Address | Interface | TTL |
|-------------|-----------|-----|
| A           | 1         | 60  |
| A'          | 4         | 60  |

- **Frame destination unknown**: If a switch doesn’t know the destination’s location, it floods the network.
- **Frame destination known**: The switch forwards the frame through the appropriate interface.

## Interconnecting Switches

- **Self-learning switches** can be connected together. When sending from **A to G** (via multiple switches), the switch network uses **self-learning** to forward the frame along the correct path. A switch need the ability to [[Isolating Traffic Patterns and Providing Multiple Access]]




