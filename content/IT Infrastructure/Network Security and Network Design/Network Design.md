---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# Network Design

## Design Goals
Good network designs should:
- **Deliver services** requested by users.
- **Ensure acceptable throughput** and response times.
- **Be within budget** and maximize cost efficiency.
- **Be reliable** and resilient.
- **Be expandable** without major redesign.
- **Be manageable** by support and maintenance staff.
- **Be well-documented** for future reference.

## Design Choices
Key factors to consider in network design include:
- **Balance of distribution**: Centralized or decentralized systems.
- **Level of transparency**: How seamless the user experience is across networks.
- **Security**: How to secure data, devices, and communications.
- **Connectivity technology**: Selecting appropriate technologies.
- **Green technology**: Emphasizing low power consumption and eco-friendliness.

## Design Approaches
There are two main methods:
- **Traditional Analytic Design**: Detailed analysis of needs and technical solutions.
- **Building Block Approach**: A modular approach where components are integrated progressively.

Both methods follow an **iterative design process**.

## The Design Process

### Design Stages - Agree Requirements
- Engage end-users to understand **business objectives** and **technical specifications**.
- Translate business goals into **phased technical requirements**.

### Design Stages - Designing Requirements
- **Complete** the design and ensure nothing is missed.
- Use a priority system:
  - **[M] Mandatory**
  - **[H] Highly desirable**
  - **[D] Desirable**
  - **[N] Note**

### Design Stages - Assessing Requirements
- Consider **costs over the network's lifecycle**, such as support, maintenance, upgrades, and project management.
- Use a **weighted matrix** system to rank suppliers, assigning higher multipliers for critical features.

### Design Stages - Information Gathering
- Collect detailed data on:
  - **User location** and behavior.
  - **Site constraints** (security, costs, traffic).
  - **Servers, WAN/backbone traffic**, and service needs.
  - Legacy systems and specific **availability needs**.
  - **Greenfield** or **existing site**.

### Design Stages - Site Constraints
- **Greenfield** sites: No legacy constraints but require simulations to predict network performance.
- **Existing** sites: Easier to assess due to observable bottlenecks but limited by current infrastructure.

### Design Stages - Planning
- Information on hosts, users, and services forms the foundation of the iterative process:
  - Conceptual design, analysis, refinement, and review.
  - Use **brainstorming**, **modelling tools**, and **design reviews**.

## Connectivity Options
- **Technology choices** include LANs (Ethernet, Token Ring), MANs (MPLS, ATM), WANs (IP routing, ISDN), and wireless options (802.11, Bluetooth, GSM).
- Factors determining the choice include:
  - **Packet, cell, or circuit switching**.
  - **Wired vs. wireless**.
  - **Distance**, **bandwidth**, **performance**, and **Quality of Service (QoS)**.

## Capacity Planning

### Capacity Planning - Outline
Capacity planning ensures:
- Minimizing **downtime**.
- Maximizing **service delivery** to users.
- Minimizing **procurement and maintenance costs**.
- Avoiding costly **upgrades** or **bad publicity** due to poor performance.

### Capacity Planning - Stages
1. **Form discussion groups** with users and stakeholders.
2. **Quantify user behavior** and location.
3. **Quantify application behavior**, performance characteristics, and impact on the network.
4. **Baseline the existing network** to analyze current performance.
5. **Make traffic projections** using tools and simulations.
6. **Summarize data** to inform the design process, considering budget, user populations, and applications.

### Good Design Principles
- Network design should be:
  - **Iterative**: Continuous refinement.
  - **Logical and consistent**.
  - Focused on **performance and cost** metrics.
  - More than just **technology selection**. It should consider user needs and system sustainability.