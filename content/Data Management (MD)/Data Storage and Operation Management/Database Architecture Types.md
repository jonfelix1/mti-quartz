---
tags:
- mandat
- note
Class: "[[Data Management Class (ManDat)]]"
Topic: "[[Data Storage and Operation Management]]"
---

# Database Architecture Types

Database architecture refers to the structure and organization of a database system. It defines how data is stored, accessed, and managed. Understanding different types of database architectures is crucial for designing systems that meet specific organizational needs.

## Types of Database Architecture

> Types of Database Architecture
> ![[Pasted image 20241015131605.png#invert_B]]


### Centralized Databases

- **Definition**: Centralized databases store all data in a single location or system.
  
- **Characteristics**:
  - All data is managed from one central point.
  - Ideal for environments where data access needs to be restricted.
  - Simplifies management and security since everything is located in one place.

- **Advantages**:
  - Easier to maintain and secure.
  - Simplified backup and recovery processes.

- **Disadvantages**:
  - Single point of failure; if the central system goes down, all data becomes inaccessible.
  - Scalability can become an issue as the volume of data grows.

### Distributed Databases

- **Definition**: Distributed databases manage multiple databases across different systems or locations.

- **Characteristics**:
  - Data is spread across various sites, which can be geographically distributed.
  - Each site can operate independently, but they are part of a larger system.

- **Types of Distributed Databases**:
  - **Federated Databases**: 
    - Comprise multiple autonomous databases that are linked to form a single database system.
    - Each database retains its autonomy while allowing for data sharing and integration without duplication.
    - Useful for organizations that need to maintain separate databases for different departments but want to provide a unified view of the data.

> Federated Databases
> ![[Pasted image 20241015131707.png#invert_B]]

  - **Non-Federated Databases**: 
    - These databases do not allow for autonomy; they are tightly coupled and rely on a central management system.
    - Typically used in scenarios where strict consistency and control are required.

- **Advantages**:
  - Enhanced reliability and availability; if one database fails, others can still function.
  - Improved performance due to localized data access.

- **Disadvantages**:
  - More complex management and maintenance compared to centralized systems.
  - Potential issues with data consistency due to the distributed nature.

### Virtualization and Cloud Platforms

- **Definition**: Virtualization platforms abstract physical hardware resources, allowing multiple virtual instances to run on a single physical machine. Cloud platforms provide services over the internet without requiring knowledge of the physical infrastructure.

- **Characteristics**:
  - Supports various database deployment options, such as Database-as-a-Service (DaaS).
  - Enables flexible resource allocation based on demand.

- **Advantages**:
  - Scalability: Easily scale resources up or down based on needs.
  - Cost-effective: Pay-as-you-go models reduce upfront costs.

- **Disadvantages**:
  - Dependency on internet connectivity and service providers.
  - Potential security concerns with sensitive data stored off-site.
