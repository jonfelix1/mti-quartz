---
tags:
- mandat
- note
Topic: "[[Data Modelling and Design]]"
Class: "[[Data Management Class (ManDat)]]"
---

# Data Modelling Schemes

Data modeling schemes are essential frameworks that help organizations structure and manage their data effectively. Each scheme has unique characteristics, components, and use cases. Below is a detailed overview of various data modeling schemes, including their definitions, components, and applications.

## Relational Modeling

### Overview
- **Origin**: Introduced by Dr. Edward Codd in 1970.
- **Purpose**: Provides a systematic way to organize data reflecting its meaning.

### Components
- **Entities**: Represent objects or concepts.
- **Attributes**: Characteristics of entities.
- **Relationships**: Connections between entities.

### Notations
- **Information Engineering (IE)**
- **Integration Definition for Information Modeling (IDEF1X)**
- **Barker Notation**
- **Chen Notation**

### Applications
Used extensively in transactional systems and applications requiring structured data storage.

## Dimensional Modeling

### Overview
- **Purpose**: Optimizes data for query performance and analysis, particularly in data warehousing scenarios.

### Components
- **Fact Tables**: Store quantitative data for analysis, typically numeric values.
- **Dimension Tables**: Contain descriptive attributes related to the facts, often textual.

### Characteristics
- Fact tables occupy a significant portion of the database (approximately 90%).
- Designed to facilitate complex queries and reporting.

## Object-Oriented Modeling (UML)

### Overview
- **Purpose**: Utilizes object-oriented principles to represent data structures as objects.

### Components
- **Objects**: Instances of classes that encapsulate both data and behavior.
- **Classes**: Define the properties and methods of objects.

### Applications
Commonly used in software engineering and applications that require complex data structures and relationships.

## Fact-Based Modeling

### Overview
- **Perspective**: Views the world in terms of objects and facts that relate to those objects.

### Characteristics
- Does not utilize attributes; instead, it expresses exact relationships between objects.
  
### Notations
- **Object Role Modeling (ORM)**
- **Fully Communication Oriented Modeling (FCO-IM)**

### Applications
Useful in scenarios where clear relationships between data points are critical without added complexity from attributes.

## Time-Based Modeling

### Overview
- **Purpose**: Associates data values with specific time values, making it suitable for historical data tracking.

### Components
- **Data Vault**: A detail-oriented, time-based set of normalized tables supporting various business functions.
  - **Hubs**: Core entities.
  - **Links**: Relationships between hubs.
  - **Satellites**: Attributes related to the hubs over time.

### Applications
Ideal for businesses needing to track changes over time, such as financial institutions or historical databases.

## NoSQL

NoSQL databases provide flexible schemas and are designed to handle large volumes of unstructured or semi-structured data. They can be categorized into several types:

### Document Stores
- Store all related information in a single document, facilitating easier access and management. 
  - Example: A single document may contain student, course, and registration information.

### Key-Value Stores
- Store data in pairs of keys and values, allowing for quick retrieval based on unique keys.

### Column-Oriented Stores
- Organize data into columns rather than rows, optimizing read performance for analytical queries.

### Graph Databases
- Represent relationships as nodes connected by edges, ideal for applications that require deep relationship mapping.
  
## Summary of Data Modeling Schemes

| Scheme                  | Key Features                                          | Use Cases                               |
|------------------------|------------------------------------------------------|-----------------------------------------|
| Relational              | Structured tables with defined relationships         | Transactional systems                   |
| Dimensional             | Fact and dimension tables for analysis               | Data warehousing                         |
| Object-Oriented         | Objects encapsulating data and behavior               | Complex software applications            |
| Fact-Based              | Focus on relationships without attributes             | Clear relationship modeling              |
| Time-Based              | Chronological associations with time values           | Historical tracking                      |
| NoSQL                   | Flexible schema types (document, key-value, etc.)    | Large-scale unstructured data           |

Each of these schemes serves specific needs within an organization's data architecture, facilitating better management, analysis, and retrieval of information. Understanding these schemes allows organizations to choose the most suitable approach based on their unique requirements.
