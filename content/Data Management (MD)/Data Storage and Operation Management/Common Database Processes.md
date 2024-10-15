---
tags:
- mandat
- note
Class: "[[Data Management Class (ManDat)]]"
Topic: "[[Data Storage and Operation Management]]"
---

# Common Database Processes

Common database processes are essential activities that ensure the effective management, integrity, and performance of databases throughout their lifecycle. These processes facilitate data handling, improve system reliability, and support organizational goals. Key processes include **archiving**, **capacity and growth projections**, **change data capture**, **purging**, **replication**, **resiliency and recovery**, **retention**, and **sharding**.

## Key Common Database Processes

### 1. Archiving

- **Definition**: Archiving involves moving inactive or less frequently accessed data from primary storage to a secondary location for long-term retention.

- **Purpose**:
  - Reduces the size of active databases, improving performance.
  - Ensures compliance with regulatory requirements for data retention.

- **Characteristics**:
  - Archived data is typically stored in a format that allows for easy retrieval.
  - May involve the use of specialized archiving solutions or services.

### 2. Capacity and Growth Projections

- **Definition**: This process involves forecasting future storage needs based on current usage trends and anticipated growth.

- **Purpose**:
  - Helps organizations plan for future storage requirements.
  - Ensures that sufficient resources are available to accommodate growth without impacting performance.

- **Characteristics**:
  - Utilizes historical data analysis and predictive modeling techniques to estimate future needs.
  - Involves collaboration between IT teams and business units to align projections with organizational goals.

### 3. Change Data Capture (CDC)

- **Definition**: CDC is a technique used to identify and capture changes made to the database in real-time or near-real-time.

- **Purpose**:
  - Facilitates data replication, synchronization, and integration processes.
  - Ensures that downstream systems have access to the most current data.

- **Characteristics**:
  - Can be implemented using triggers, database logs, or specialized CDC tools.
  - Supports both incremental updates and full data refreshes.

### 4. Purging

- **Definition**: Purging involves the systematic removal of obsolete or unnecessary data from the database.

- **Purpose**:
  - Helps maintain optimal database performance by freeing up storage space.
  - Reduces clutter and improves data quality by ensuring that only relevant information is retained.

- **Characteristics**:
  - Typically follows established retention policies and compliance requirements.
  - May involve automated scripts or manual processes to identify and delete data.

### 5. Replication

- **Definition**: Replication is the process of copying and maintaining database objects in multiple locations for redundancy and availability.

> Replication
> ![[Pasted image 20241015131853.png#invert_B]]

- **Types of Replication**:
  - **Mirroring**: Updates to the primary database are immediately replicated to a secondary database as part of a two-phase commit process.
  
  - **Log Shipping**: A secondary server receives copies of transaction logs from the primary database at regular intervals.

- **Purpose**:
  - Enhances data availability and disaster recovery capabilities.
  
- **Characteristics**:
  - Can be configured for synchronous or asynchronous operations depending on business needs.

### 6. Resiliency and Recovery

- **Definition**: This process involves planning for system failures and ensuring that data can be restored quickly after an incident.

- **Types of Recovery**:
  - **Immediate Recovery**: Automatic resolution of issues, often through design features.
  
  - **Critical Recovery**: Aimed at restoring functionality as quickly as possible to minimize downtime.
  
  - **Non-Critical Recovery**: Restoration can be delayed until more critical systems are back online.

- **Purpose**:
  - Ensures business continuity and minimizes operational disruptions during failures.

### 7. Retention

- **Definition**: Data retention refers to policies governing how long different types of data should be stored before being deleted or archived.

- **Purpose**:
  - Complies with legal, regulatory, and organizational requirements regarding data management.
  
- **Characteristics**:
  - Involves categorizing data based on its importance, sensitivity, and usage frequency.
  
### 8. Sharding

- **Definition**: Sharding is the process of partitioning a large database into smaller, more manageable pieces called shards, which are distributed across multiple servers.

- **Purpose**:
  - Improves performance by allowing parallel processing of queries across shards.
  
- **Characteristics**:
  - Each shard operates independently but contributes to a unified view of the entire dataset.
  