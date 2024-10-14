---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Forwarding Table

- The **forwarding table** displays routes and can be viewed using the command: `netstat -rn`. Sometimes it’s also called the **routing table**.

## Forwarding Table Structure

- **Destination**: Can be a **host address** or **network address**. If the **'H' flag** is set, it indicates a host address.
- **Gateway**: The **next hop IP address** or router. The **'G' flag** shows whether the destination is directly connected or not.
- **Flags**:
    - **U flag**: Is the route up?
    - **G flag**: Router (indirect vs direct connection).
    - **H flag**: Host (indicates whether the destination is a host or network address).
