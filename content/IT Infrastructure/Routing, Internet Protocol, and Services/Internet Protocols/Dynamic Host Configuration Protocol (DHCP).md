---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Dynamic Host Configuration Protocol (DHCP)
- **DHCP** facilitates the dynamic assignment of IP addresses to devices on a network, optimizing the use of available IP addresses.
- **Static vs. Dynamic Assignment**: IP addresses can be assigned statically (permanently) or dynamically. Dynamic assignment allows for more efficient utilization of the limited pool of available addresses.
- **Process**: When a DHCP client requests an IP address, the DHCP server checks its static table for existing entries. If none are available, it assigns an IP from its pool of available addresses.
- **Lease Duration**: The DHCP server assigns IP addresses temporarily, specifying a lease duration. The default lease time is often one hour, but clients can request renewal before expiration.
