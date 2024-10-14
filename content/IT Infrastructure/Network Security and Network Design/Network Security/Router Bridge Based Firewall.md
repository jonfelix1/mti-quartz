---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# Router/Bridge Based Firewall

- **Definition**: A router/bridge based firewall is a security device that operates on a network router or bridge to monitor and control incoming and outgoing network traffic. It serves to protect a network from unauthorized access and various cyber threats.
    
- **Functionality**:
    
    - Operates at the network layer (Layer 3) of the OSI model.
    - Filters traffic based on IP addresses and ports.
    - Can protect multiple devices within a network segment.
- **Key Features**:
    
    - **Packet Filtering**: Analyzes packets of data and allows or blocks them based on predefined security rules.
    - **Network Address Translation (NAT)**: Hides internal IP addresses by translating them into a single external IP address.
    - **Stateful Inspection**: Tracks the state of active connections and makes decisions based on the context of the traffic.
- **Cisco Firewalls**: Many routers from Cisco come with built-in firewall features integrated into their IOS operating system, providing added security for networks.
    
- **Advantages**:
    
    - Protects a wide range of devices connected to the network.
    - Can be configured to respond to specific types of traffic.
    - Helps in segmenting network traffic for improved security.
- **Considerations**:
    
    - Requires proper configuration to ensure effective protection.
    - May have limitations in detecting certain types of threats compared to more advanced firewalls.

This type of firewall is essential for managing network security at a broader level, providing foundational protection against a variety of threats.