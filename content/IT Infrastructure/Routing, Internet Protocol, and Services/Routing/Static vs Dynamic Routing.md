---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Static vs Dynamic Routing

- **Static Routing:**
    
    - Forwarding table entries are manually configured by an administrator.
    - **Advantages:**
        - Provides more control.
        - Can be used for non-destination-based forwarding.
    - **Disadvantages:**
        - Doesn't scale well.
        - Slow to adapt to network changes.
- **Dynamic Routing:**
    
    - Routers use routing protocols to exchange network information and compute the best routes.
    - **Advantages:**
        - Adapts quickly to changes in network topology.
        - Scalable for large networks.
    - **Disadvantages:**
        - Complex distributed algorithms.
        - Higher resource consumption (CPU, bandwidth, memory).
        - Difficult to debug.
