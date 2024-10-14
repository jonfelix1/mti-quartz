---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Basic Dynamic Routing Methods

Dynamic routing methods determine how routes are calculated and updated in a network. These methods adjust routes based on changing network conditions without requiring manual configuration. The three key dynamic routing methods are **source-based routing**, **link-state routing**, and **distance vector routing**.

---

## Source-Based Routing

In source-based routing, the **source node** has the full responsibility for finding the route to the destination. The source node typically receives a **complete map** of the network and uses this map to compute the best route.

- **Route Setup**: The source either signals the route setup (as in ATM networks) or encodes the entire route into the packet header, which is generally inefficient due to extra overhead.
- **Route Encoding**: The computed route is added to the packet, so the intermediate routers do not have to compute the path, but instead follow the path provided by the source.

### Advantages:
- Centralized control: The source has a full view of the network topology.
- Can optimize routes based on specific policies or requirements.

### Disadvantages:
- Scalability issues in large networks due to the overhead of encoding full paths.
- Inefficient when network conditions change dynamically, as the source would need frequent updates on the network's state.

---

## Link-State Routing

In link-state routing, every node (router) has a complete view of the network's topology. The nodes exchange **link-state information** with their neighbors, and each node computes the best next hop for every destination based on the received data. [[Link-State Algorithm (SPF)]]

- **Network Map**: Each node independently builds a full map of the network based on the link-state information.
- **Local Computation**: Using algorithms like **Dijkstra's algorithm** as written in [[Routing Example]], nodes compute the **shortest path** from themselves to every destination.
- **Consistency**: Since all nodes have the same information, their next-hop decisions are consistent across the network.

### Advantages:
- **Fast convergence**: Nodes quickly recompute routes when network topology changes.
- **Efficient routing**: Provides an optimal path based on real-time network conditions.

### Disadvantages:
- High resource consumption (CPU, memory) to store and process the entire network map.
- Frequent updates can lead to increased bandwidth usage, especially in large networks.

---

## Distance Vector Routing

In distance vector routing, routers share information only about their **directly connected neighbors**. Each node maintains a **distance vector** that provides the shortest distance (in terms of hops or cost) to each destination.

- **Distance Signposts**: Nodes set up "signposts" indicating the distance to each possible destination.
- **Iterative Process**: The nodes exchange distance vectors with their neighbors, updating their own distance vectors based on the neighbors' information. This process continues until the network converges.
- **Bellman-Ford Algorithm**: The distance vector algorithm is often based on the **Bellman-Ford algorithm**, which calculates the shortest paths iteratively.

### Key Concepts:
- **Consistency Condition**: The distance to a destination is updated using the formula:
$$
  D(i,j) = c(i,k) + D(k,j)
$$
  Where:
  - $D(i,j)$ is the distance from node $i$ to destination $j$,
  - $c(i,k)$ is the cost from node $i$ to neighbor $k$,
  - $D(k,j)$ is the distance from $k$ to $j$.

- **Next-Hop Value**: In addition to the distance, nodes also store the next-hop for each destination, indicating the neighbor through which the packet should be forwarded.

### Advantages:
- **Simple**: Easy to implement and requires little computation.
- **Low overhead**: Nodes only share information with neighbors, reducing the complexity of routing updates.

### Disadvantages:
- **Count to infinity problem**: Bad news (e.g., link failures) travels slowly, causing incorrect routing information to propagate.
- **Slow convergence**: Distance vector protocols can take a long time to converge, especially in large or dynamic networks.

### Optimizations:
- **Poisoned Reverse**: A method to mitigate the **count to infinity problem**. If a node routes to a destination via a neighbor, it tells that neighbor that the distance to the destination is infinite, preventing the neighbor from routing back through that node.

# Conclusion

Both link-state and distance vector routing methods are widely used in modern networks, with link-state being more appropriate for large, complex networks due to its ability to quickly adapt to changes. Distance vector routing, while simpler, is less efficient in dynamic environments due to its slower convergence and potential issues like the count-to-infinity problem.
