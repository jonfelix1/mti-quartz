---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Hub vs Switch vs Router

- **Hub**:
    - Operates at Layer 1 of [[Forwarding Table Layer]] and simply broadcasts signals. It has no forwarding table and doesn't filter traffic.
- **Switch**:
    - Operates at Layer 2 of [[Forwarding Table Layer]] with L2 forwarding tables built using dynamic learning algorithms.
    - Switches send packets only to the destination's segment.
    - They limit broadcasts and collisions within collision domains and use flooding if the destination address is unknown.
- **Router**:
    - Operates at Layer 3 of [[Forwarding Table Layer]]using L3 forwarding tables.
    - Routers use distributed protocols to learn about network topology and never broadcast if a route is unknown. They delegate to other routers for further routing.

