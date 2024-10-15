---
tags:
- mandat
- note
Class: "[[Data Management Class (ManDat)]]"
Topic: "[[Data Storage and Operation Management]]"
---

# Data Processing Types

Data processing types are essential frameworks that define how data is handled within database systems. Understanding these processing types helps organizations manage their data effectively, ensuring reliability, availability, and performance. The primary data processing types include **ACID**, **BASE**, and the **CAP theorem**.

> Data Processing Types
> ![[Pasted image 20241015131759.png#invert_B]]

## ACID Properties

ACID stands for **Atomicity**, **Consistency**, **Isolation**, and **Durability**. These properties are fundamental for ensuring reliable transactions in relational databases.

### Atomicity

- **Definition**: Guarantees that a transaction is treated as a single, indivisible unit. Either all operations within the transaction are completed successfully, or none are applied.
  
- **Importance**: Prevents partial updates to the database, ensuring that the system remains in a consistent state.

### Consistency

- **Definition**: Ensures that a transaction brings the database from one valid state to another, maintaining all predefined rules and constraints.
  
- **Importance**: Protects data integrity by enforcing rules such as foreign key constraints and unique constraints.

### Isolation

- **Definition**: Ensures that concurrently executed transactions do not interfere with each other. Each transaction must appear isolated from others.
  
- **Importance**: Prevents issues like dirty reads, non-repeatable reads, and phantom reads, which can lead to inconsistent data states.

### Durability

- **Definition**: Guarantees that once a transaction has been committed, it will remain so even in the event of a system failure.
  
- **Importance**: Ensures that completed transactions are saved permanently, typically through mechanisms like logging and backup systems.

## BASE Properties

BASE is an acronym for **Basically Available**, **Soft State**, and **Eventual Consistency**. This model is often applied in distributed systems, particularly in big data environments.

### Basically Available

- **Definition**: The system guarantees some level of availability to data even during node failures. While responses may be stale, the system continues to provide access.
  
- **Importance**: Ensures that users can still interact with the system even when parts of it are down.

### Soft State

- **Definition**: Indicates that the state of the system may change over time, even without new input. Data may not be current or consistent at all times.
  
- **Importance**: Acknowledges that distributed systems operate under conditions where data can be in flux.

### Eventual Consistency

- **Definition**: Guarantees that all updates will propagate throughout the system eventually, leading to a consistent state across all nodes.
  
- **Importance**: Allows for temporary inconsistencies while ensuring long-term reliability and consistency.

## CAP Theorem

> CAP Theorem
> ![[Pasted image 20241015131826.png#invert_B]]

The CAP theorem states that in a distributed data store, it is impossible to simultaneously guarantee all three of the following properties:

1. **Consistency**: Every read receives the most recent write or an error.
   
2. **Availability**: Every request receives a response (success or failure), regardless of the state of any individual node.

3. **Partition Tolerance**: The system continues to operate despite arbitrary partitioning due to network failures.

### Trade-offs

- In practice, systems must choose two out of these three properties:
  - CP (Consistency and Partition Tolerance): Systems may sacrifice availability during network partitions.
  - AP (Availability and Partition Tolerance): Systems may return stale data when consistency cannot be guaranteed.
