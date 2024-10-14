---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Routing Classification

Routing in computer networks can be broadly classified into two major categories: **Intradomain Routing** and **Interdomain Routing**. Each of these classifications serves different purposes and operates with distinct protocols and goals. Below is a detailed explanation of both.

---

## 1. Intradomain Routing

**Intradomain routing**, also known as **Interior Gateway Protocols (IGP)**, is concerned with routing within a **single autonomous system (AS)**. An autonomous system is a network or collection of networks under a common administration that presents a unified routing policy to the outside world.

### Objectives of Intradomain Routing
- The main goal is to find the **shortest or most efficient path** between nodes (routers) within the AS.
- Efficient management of network traffic, ensuring the fastest possible communication within the system.
- Achieving **fast convergence** when topology changes occur, such as link failures or new routers being added.
  
### Characteristics of Intradomain Routing
- **Limited to a single AS**: The protocol only works within one administrative domain, where all routers trust each other.
- **Optimizes for path efficiency**: The goal is to ensure that data travels via the shortest or least-cost path.
- **Can scale from small networks to large ISPs**: Different protocols can handle networks of various sizes, from a few routers in small enterprises to thousands of routers in large ISPs.
  
### Common Intradomain Routing Protocols
- **OSPF (Open Shortest Path First)**: A widely used protocol that finds the shortest path using **link-state routing**. All routers maintain a full map of the network topology and use it to compute the shortest path.
- **RIP (Routing Information Protocol)**: An older protocol that uses **distance-vector routing**, where routers share information with neighbors about the best route to a destination.
- **IS-IS (Intermediate System to Intermediate System)**: Another link-state protocol, similar to OSPF, but used primarily in large ISP networks.

### Requirements for Intradomain Routing
- **Scalability**: The protocol must be scalable enough to handle both small networks with a few routers and large networks with thousands of routers.
- **Fast Convergence**: In large-scale networks, fast convergence is critical, especially in enterprise and ISP environments where disruptions must be minimized.
  - Small networks can tolerate occasional connectivity disruptions, but large networks (e.g., ISPs) require rapid adaptation to topology changes.
- **Operational Simplicity**: For smaller networks, the protocol should be **self-configuring**, but larger networks need more operational controls for administrators to fine-tune routing behavior.
- **Traffic Engineering**: Large networks often need advanced **traffic engineering** capabilities to manage congestion and optimize performance.

---

## 2. Interdomain Routing

**Interdomain routing**, also known as **Exterior Gateway Protocols (EGP)**, manages routing between **multiple autonomous systems**. It allows different networks, each under separate administrative control, to communicate with each other. The Internet is built upon thousands of autonomous systems, and interdomain routing is essential for connecting them.

### Objectives of Interdomain Routing
- **Reachability, not optimality**: The focus is on ensuring that data can reach its destination, not necessarily on finding the shortest path.
- **Policy-driven routing**: Interdomain routing must adhere to the **routing policies** defined by each AS, which may not always align with the shortest path.
  - Policies are often dictated by **business relationships**, such as **peering agreements** or **service level agreements (SLAs)**.
- **Scalability for global networks**: Interdomain routing must scale to support the entire Internet, which consists of millions of networks and routes.

### Characteristics of Interdomain Routing
- **Multiple ASes involved**: Routes often span multiple autonomous systems, requiring coordination between different administrative entities.
- **Focus on policies and business relationships**: Unlike intradomain routing, which focuses on technical efficiency, interdomain routing is driven by **business decisions**. For example, an AS might prefer to send traffic through a partner network rather than the shortest path.
- **Global scale**: The protocol must be able to handle the size and complexity of the global Internet, with millions of routes to manage.

### Common Interdomain Routing Protocols
- **BGP (Border Gateway Protocol)**: The primary interdomain routing protocol on the Internet. BGP allows ASes to exchange routing information and make policy-based routing decisions.
  - **Policy-based routing**: BGP allows each AS to define routing policies based on business agreements, such as prioritizing certain routes or avoiding certain networks.
  - **Path Vector Protocol**: BGP uses the **path vector** method, where each router maintains the path (sequence of ASes) a route has taken. This ensures **loop avoidance**.
- **EGP (Exterior Gateway Protocol)**: The predecessor to BGP, EGP is rarely used today but laid the foundation for interdomain routing on the Internet.

### Requirements for Interdomain Routing
- **Scalability**: Interdomain routing protocols need to scale to handle the entire global Internet, supporting millions of routes and routing table entries.
- **Address Aggregation**: To minimize the size of routing tables, **address aggregation** techniques (such as **CIDR - Classless Inter-Domain Routing**) are used to combine smaller IP address blocks into larger ones.
- **Policy Flexibility**: The protocol must allow each AS to implement flexible, **policy-based routing**. These policies dictate how traffic should be routed based on business relationships or security concerns.
- **Focus on reachability**: The goal is to ensure connectivity between autonomous systems, regardless of whether the path is optimal or efficient.
- **Topology Flexibility**: Interdomain routing must be flexible enough to support various topologies, not restricted to specific structures like trees or meshes.

---

## Key Differences Between Intradomain and Interdomain Routing

| **Aspect**               | **Intradomain Routing (IGP)**                            | **Interdomain Routing (EGP)**                         |
|--------------------------|----------------------------------------------------------|-------------------------------------------------------|
| **Scope**                | Within a single autonomous system (AS)                   | Between multiple autonomous systems (ASes)            |
| **Objective**            | Shortest path, efficiency within a single AS             | Reachability between ASes, policy-driven routing       |
| **Control**              | Centralized control within an AS                         | Decentralized control between ASes                    |
| **Routing Protocols**    | OSPF, RIP, IS-IS                                         | BGP                                                   |
| **Routing Decision**     | Based on link costs or hop counts                        | Based on business policies and AS relationships       |
| **Routing Algorithm**    | Typically shortest-path first (link-state or distance-vector) | Path-vector (BGP), based on policies                   |
| **Convergence Speed**    | Fast convergence required                                | Slower convergence acceptable for inter-AS traffic     |
| **Addressing**           | Primarily deals with host or subnet addressing           | Address aggregation through CIDR                      |
| **Scale**                | Handles smaller networks (up to thousands of routers)    | Handles global networks, scalable to millions of routes|
| **Policy**               | Minimal policy, focuses on efficiency                    | Extensive policy, influenced by business relationships |

---

## Examples of Routing Use Cases

- **Intradomain Routing**: Used within a company’s internal network or an ISP’s network. For instance, a small business with several routers in different buildings may use OSPF to ensure that all internal devices can communicate efficiently.

- **Interdomain Routing**: Used for communication across different networks, such as between an ISP and another ISP, or between an enterprise network and its upstream provider. BGP ensures that traffic can travel from one AS to another, respecting the routing policies defined by each AS.

---

## Overview

**Intradomain routing** focuses on **optimizing the path** within a single AS for performance, using protocols like **OSPF** and **RIP**, while **Interdomain routing** focuses on **policy-driven decisions** across ASes, relying heavily on **BGP** for global Internet connectivity. Each plays a crucial role in ensuring data reaches its destination efficiently and according to the goals of the network administrators.