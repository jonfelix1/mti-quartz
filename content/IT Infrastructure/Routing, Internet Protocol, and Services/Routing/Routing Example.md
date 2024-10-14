---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Routing Examples

In computer networks, **routing algorithms** play a critical role in determining the best path for data packets to travel from a source to a destination. Here we will elaborate on two widely used routing algorithms: **Distance Vector (Bellman-Ford)** and **Link-State (Dijkstra’s Algorithm)**. These methods differ in how they manage network topology information and how they calculate the best routes.

---

## 1. Distance Vector Routing (Bellman-Ford Algorithm)

**Distance Vector Routing** is a decentralized approach where each router only has information about its **direct neighbors**. Over time, routers exchange this information, building up a complete view of the network’s best paths.

### Key Concepts:
- **Distance Vector**: A table maintained by each router that contains the **distance to every destination**.
- **Next-Hop**: In addition to the distance, each router stores the **next-hop neighbor** to forward packets to, for each destination.

### Bellman-Ford Algorithm:
The algorithm is based on the idea that the shortest path from node $i$ to node $j$ can be recursively determined if node $i$ knows the shortest path from one of its neighbors $k$ to $j$, plus the direct cost between $i$ and $k$.

- The formula for this recursive calculation is:
  $$
  D(i,j) = \min \{ c(i,k) + D(k,j) \}
  $$
  Where:
  - $D(i,j)$ is the distance from node $i$ to destination $j$,
  - $c(i,k)$ is the link cost from node $i$ to its neighbor $ k $,
  - $D(k,j)$ is the distance from $k$ to $j$, as known by neighbor $k$.

### Example:

Consider the following network with five nodes $(A, B, C, D, E)$ and the following link costs:

```mathematica
A — 7 — B
|       |
1       2
|       |
E — 1 — D
|       |
8       3
|       |
C —————
```

1. **Initial Distance Values**:
   - **Node A**: $[0, 7, \infty, \infty, 1]$
     - $D(A,A) = 0$ (distance to itself),
     - $D(A,B) = 7$ (direct link),
     - $D(A,C) = \infty$ (not connected directly),
     - $D(A,D) = \infty$ (not connected directly),
     - $D(A,E) = 1$ (direct link).

2. **After Iteration 1**:
   - Node A exchanges distance vectors with its neighbors (B, E).
   - A learns that $D(B,D) = 2$ and updates $D(A,D) = 3$ via E (since $D(A,E) + D(E,D) = 1 + 2 = 3$).
   - Updated distance vector for A: $[0, 7, \infty, 3, 1]$.

3. **After Iteration 2**:
   - Further exchanges result in an update of $D(A,C)$ to 8, as A learns from E that $D(E,C) = 8$.
   - Updated distance vector for A: $[0, 7, 8, 3, 1]$.

4. **Convergence**:
   - After further iterations, the algorithm converges, and the final shortest paths are calculated, such as $D(A,B) = 6$, $D(A,C) = 5$, and so on.

### Problems:
- **Count-to-Infinity Problem**: When a link fails, incorrect distance values may propagate slowly, leading to incorrect paths being used for a long time.
- **Poisoned Reverse**: A method to prevent loops by marking routes as "infinite" to neighbors, signaling that the route should not be used.

---

## 2. Link-State Routing (Dijkstra’s Algorithm)

In **Link-State Routing**, each router has a complete view of the network's topology. This is achieved by routers exchanging **link-state advertisements (LSAs)**, which describe the status of their links. Once all routers have this information, they each compute the **shortest path** to every destination independently using Dijkstra’s algorithm.

### Key Concepts:
- **Link-State Database**: Each router stores a map of the entire network, including the status (cost, availability) of each link.
- **Shortest Path Tree (SPT)**: Using Dijkstra's algorithm, each router computes the shortest path to every other router, which forms a tree structure rooted at itself.

### Dijkstra’s Algorithm:
The algorithm finds the shortest path from a source node to every other node in the network. It works by progressively **expanding the shortest known path** from the source node, updating distances to other nodes along the way.

### Steps:
1. **Initialize**: Set the distance to the source node to 0 and all other nodes to infinity. Mark all nodes as unvisited.
2. **Visit Neighbors**: Start at the source node. For each unvisited neighbor, calculate the tentative distance (current distance + link cost).
3. **Update**: If the new tentative distance is smaller than the previously known distance, update the distance.
4. **Move to Next Node**: Select the unvisited node with the smallest tentative distance, mark it as visited, and repeat the process until all nodes are visited.

### Example:

Using the same network as before:

```mathematica
A — 7 — B
|       |
1       2
|       |
E — 1 — D
|       |
8       3
|       |
C —————
```

1. **Initialization**:
   - Start from node **A**. Initialize distances: $[0, \infty, \infty, \infty, \infty]$.
   - Set $D(A,A) = 0$, $D(A,E) = 1$, and $D(A,B) = 7$.

2. **Step 1**: 
   - Visit node **E** (the neighbor with the smallest tentative distance, 1).
   - Update distances: $D(A,D) = 1 + 2 = 3$.

3. **Step 2**: 
   - Visit node **D** (tentative distance 3).
   - Update distances: $D(A,C) = 3 + 3 = 6$.

4. **Step 3**:
   - Visit node **C** (tentative distance 6).
   - Update distances: No further updates are needed since C has no new neighbors.

5. **Final Shortest Paths**:
   - From **A**: D(A,E) = 1 $, $ D(A,D) = 3 $, $ D(A,C) = 6 $, $ D(A,B) = 6$.

### Advantages:
- **Fast Convergence**: Since all routers have a consistent view of the network, routes can be recalculated quickly when the topology changes.
- **Optimal Path**: The algorithm guarantees that the computed paths are the shortest in terms of cost.

### Drawbacks:
- **High Resource Usage**: Requires more memory and processing power, as each router must maintain a full map of the network.
- **Frequent Updates**: Network-wide updates may consume significant bandwidth, especially in large and dynamic networks.

