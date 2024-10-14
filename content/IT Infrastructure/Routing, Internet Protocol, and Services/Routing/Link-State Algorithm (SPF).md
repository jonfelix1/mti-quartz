---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Link-State Algorithm (SPF)

The **Link-State Algorithm**, also known as the Shortest Path First (SPF) algorithm, is a widely used routing technique in networking. It allows routers to compute the best paths for data packets to travel from source to destination based on a comprehensive view of the network topology.

## Input and Output

### Input
1. **Link-State Advertisements (LSAs)**: Each router sends and receives LSAs containing:
   - **Router ID**: Identifier of the router.
   - **Link Cost**: Cost associated with each link (interface) to its neighbors.
   - **Neighboring Routers**: Information about directly connected routers and their respective costs.

2. **Topology Information**: Each router gathers information about the state and cost of links to all its directly connected neighbors. This information is then flooded throughout the network, allowing all routers to have a consistent view of the network topology.

### Output
1. **Shortest Path Tree (SPT)**: Each router computes a Shortest Path Tree rooted at itself, determining the shortest path to every other router in the network.

2. **Routing Table**: Based on the SPT, each router generates a routing table that contains:
   - **Destination**: The address of the destination router.
   - **Next Hop**: The next router on the path to the destination.
   - **Cost**: The total cost of reaching the destination from the source.

---

## Cost Metric Assignment

The choice of link cost plays a significant role in routing decisions, impacting traffic load distribution and network performance.

### Considerations for Assigning Cost Metrics
- **Traffic Load**: The cost metric influences the probability that a link will be part of the Shortest Path Tree (SPT). 
  - **Low Cost**: High probability that the link will attract traffic.
  - **High Cost**: Less likely to be used, which can help balance traffic loads.

### Tradeoffs
- **Convergence vs. Load Distribution**: Finding the right balance between quickly converging on routing paths and effectively distributing traffic load.
- **Avoid Oscillations**: Cost metrics should be set to prevent routing loops and instability in the network.

### Types of Metrics
1. **Static Metrics**: 
   - Based on weighted hop counts.
   - Do not account for current traffic load or demand, which can lead to inefficient routing under varying traffic conditions.

2. **Dynamic Metrics**:
   - Adjust costs based on real-time factors such as queue length or delay.
   - Can lead to oscillations and instability due to rapid changes in link states (as experienced in DARPAnet).

3. **Quasi-Static Metrics**:
   - Reassign static metrics based on overall network load, utilizing a demand matrix.
   - Assumes the network load is quasi-stationary, balancing between static and dynamic approaches.

---

## Algorithm Operation

1. **Flooding Topology Information**: 
   - Each router broadcasts its LSA to all other routers within the routing domain, ensuring a consistent view of the network topology.

2. **Local Computation**:
   - Each router computes the best end-to-end paths locally based on the received topology information.

3. **Next-Hop Determination**:
   - Each router chooses the best next-hops for each destination based on the minimized distance (cost).

### Types of Routing Protocols

1. **OSPF (Open Shortest Path First)**:
   - Utilizes link-state routing and SPF to determine the best paths.
   - Requires shared and uniform policies across the routing domain.

2. **IS-IS (Intermediate System to Intermediate System)**:
   - Another link-state protocol that operates similarly to OSPF.

3. **RIP (Routing Information Protocol)**:
   - A distance vector protocol that uses hop count as a routing metric, not requiring a detailed understanding of network topology.

4. **BGP (Border Gateway Protocol)**:
   - A path vector protocol used for inter-domain routing, which selects paths based on policy rather than minimizing distance.

---

## Conclusion

The Link-State Algorithm is a robust and efficient method for determining the best routing paths in a network. By using LSAs and computing the Shortest Path Tree, routers can make informed routing decisions that minimize delays and optimize traffic distribution. The careful assignment of cost metrics is crucial for balancing convergence speed and load distribution across the network.