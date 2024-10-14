---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Telephony Routing vs Internet Routing

---

## Telephony Routing

### Circuit-Switched Nature
- **Telephony routing** is based on **circuit-switched networks**, where a dedicated communication path (circuit) is established between two endpoints before any data (voice) transmission occurs.
- The circuit is **reserved** for the duration of the call, guaranteeing a consistent and dedicated bandwidth.
- Once the call ends, the circuit is **released** and can be used by other communications.

### Hierarchical Structure
- Telephony networks use a **3-level hierarchy**:
  - **Local Exchange Carriers (LECs)** manage local calls and direct traffic within the same geographic area.
  - **Toll switches** handle long-distance calls, determining whether to send the call over a **one-hop or two-hop path** between toll switches.
  - The **core network** is fully connected, consisting of central switches that route calls across long distances.

### Routing Algorithm
- Calls are routed based on **proximity** and resource availability:
  - If the call is within the same **Central Office (CO)**, it is directly connected.
  - If it's within the same **Local Exchange Carrier (LEC)** but across different COs, a **one-hop path** is used.
  - If it's an external call, the **toll switch** determines the optimal route. If the direct route is unavailable, a **two-hop path** is selected.

### Resource Reservation
- **Resource reservation** is fundamental to telephony routing. This includes:
  - Reserving a **64 kbps** channel for each voice connection.
  - **Signaling protocols** are used to set up, maintain, and tear down the connection.
  - The path and the required resources (bandwidth) are reserved simultaneously, ensuring no packet loss or jitter.
  
### Stable Network Topology
- The telephony network is designed for **voice traffic**, which is highly predictable and stable throughout the day.
- **Load balancing** is planned in advance based on expected call volumes at different times.
- Network routes and resources are **pre-planned**, and routes can be chosen optimally in advance because the network topology changes very little.

### Technology and Economic Aspects
- **Extremely reliable switches** ensure minimal downtime, typically less than a few minutes per year.
- The system was built with **dumb end-systems** (phones) because computing power was limited in early telephony networks, so all intelligence was placed in the network.
- The network's reliability is driven by its components' reliability, which ensures **continuous service**.

### Centralized Control
- The telephony network is often controlled by a **single organization** (e.g., AT&T for the US).
- This control allows **global optimization** of routing and network usage, as the organization can collect statistics and implement changes across the entire network.

---

## Internet Routing

### Packet-Switched Nature
- **Internet routing** is based on **packet-switched networks**, where data is broken into smaller packets that are transmitted independently across the network.
- Unlike telephony, **no dedicated path** is established before communication; instead, each packet may follow a different route to the destination.
- Packet-switched networks are designed for **data communication**, where paths can change dynamically based on network conditions.

### Decentralized and Dynamic Structure
- The Internet is built on a **decentralized model**, meaning there is no single organization that controls the entire network.
- It consists of many **autonomous systems (AS)** that interconnect with each other through **peering agreements**.
- Routing decisions are made using **distributed algorithms** (e.g., BGP, OSPF), and the network topology can change frequently.

### Routing Algorithm
- Routing on the Internet uses dynamic **distributed protocols** to compute the best paths based on factors such as **hop count**, **link costs**, and **congestion**.
- Internet routing is **policy-driven**, especially between autonomous systems. This means that routes may not always be the shortest but are determined by **business relationships** and **agreements** between networks.

### No Resource Reservation
- The Internet does not reserve resources like telephony. Instead, packets are sent whenever the network has capacity.
- This means that **packet loss, jitter, and delays** can occur during periods of high traffic.
- While **Quality of Service (QoS)** techniques can be used to prioritize certain types of traffic (e.g., voice or video), there is no **guaranteed bandwidth** as in telephony routing.

### Unreliable and Changing Topology
- Internet components (e.g., routers, links) are **cheap** and **unreliable** compared to telephony networks.
- As a result, the **topology changes frequently** due to link failures, congestion, or other issues.
- The Internet needs **dynamic routing** to continuously adapt to these changes, ensuring that packets can still find a route to their destination.

### Technology and Economic Aspects
- The Internet was originally an overlay on top of the **telephone infrastructure** and has since evolved into a global communication network.
- The use of **cheap and unreliable components** made it affordable for many entities to interconnect their **local networks** and build the global Internet.
- Because the Internet is built on top of multiple **administrative domains** (autonomous systems), each domain manages its own internal routing while participating in global routing.

### Decentralized Control
- The Internet operates with **multiple independent organizations**, each controlling its part of the network.
- This leads to **multiple routing policies** and the need for protocols like **BGP** to manage routing between different organizations.
- Internet routing is less optimized than telephony because **global optimization** is challenging when control is spread across different entities.

---

# Key Differences

| Feature                    | **Telephony Routing**                        | **Internet Routing**                                |
|----------------------------|----------------------------------------------|----------------------------------------------------|
| **Network Type**            | Circuit-switched                             | Packet-switched                                   |
| **Connection Setup**        | Requires **connection setup** before transmission | No connection setup; packets routed individually    |
| **Routing Algorithm**       | Static or semi-static, hierarchical          | Dynamic, distributed algorithms                    |
| **Resource Reservation**    | Resources (e.g., bandwidth) are reserved     | No resource reservation, best-effort transmission  |
| **Reliability**             | Highly reliable, minimal downtime            | Less reliable, frequent topology changes           |
| **Topology**                | Stable, predictable traffic                  | Dynamic, frequent changes                          |
| **Control**                 | Centralized (single organization)            | Decentralized (many independent networks)          |
| **Policy**                  | Less flexibility; focus on efficiency        | Policy-driven, influenced by business relationships|
| **Use Case**                | Voice communication                         | Data communication, multimedia, web services       |

Telephony routing is highly **centralized, reliable, and predictable**, designed for stable voice traffic, while Internet routing is **decentralized, dynamic, and flexible**, designed to handle the **unpredictability** of modern data communication across a global, heterogeneous network.