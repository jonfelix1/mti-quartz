---
tags:
- mandat
- topic
- note
Class: "[[Data Management Class (ManDat)]]"
Topic: "[[Data Architecture]]"
---

# Data Model Layers

Data modelling is a crucial aspect of data management that involves creating abstract representations of data structures. A layered approach to data modeling helps organize these representations into distinct levels, each serving specific purposes and audiences. Typically, there are three main layers in data modelling:

1. **Conceptual Data Model**
2. **Logical Data Model**
3. **Physical Data Model**

Each layer has its own characteristics, focuses on different aspects of data, and serves various stakeholders.

## Layers

---

### 1. Conceptual Data Model

#### Definition

The **Conceptual Data Model** is an abstract representation that outlines the high-level structure of the data without delving into the specifics of how it will be implemented. It focuses on defining the entities, their attributes, and relationships in a way that is understandable to business stakeholders.

#### Purpose

- Provides a high-level overview of the data landscape within the organization.
- Facilitates communication between technical and non-technical stakeholders by using familiar business terminology.
- Helps identify key business entities and their relationships.

#### Components

- **Entities**: Core business objects (e.g., Customer, Order, Product).
- **Attributes**: Characteristics of the entities (e.g., Customer ID, Order Date).
- **Relationships**: Connections between entities (e.g., a Customer places an Order).
- **Super-types/Sub-types**: Class hierarchies that categorize entities (e.g., Employee as a super-type with sub-types like Full-time and Part-time).

#### Characteristics

- **Business-Focused**: Uses terms and concepts familiar to the business.
- **Abstract and High-Level**: Avoids technical details; emphasizes relationships and interactions.
- **Documentation**: Provides definitions, examples, and distinctions between similar terms.

---

### 2. Logical Data Model

#### Definition

The **Logical Data Model** builds upon the conceptual model by adding more detail while remaining independent of any specific database or technology. It focuses on the data's logical structure and how it will be used in applications.

#### Purpose

- Provides a more detailed representation of the data, including data types and constraints.
- Serves as a bridge between the conceptual model and the physical model.
- Ensures that the data meets business requirements without getting bogged down by implementation specifics.

#### Components

- **Entities and Attributes**: More detailed than in the conceptual model, including data types and constraints.
- **Primary and Foreign Keys**: Identification of unique records and relationships between tables.
- **Normalization**: Structure the data to reduce redundancy and ensure integrity.
- **Relationships**: Defined with cardinality (e.g., one-to-many, many-to-many).

#### Characteristics

- **Data Type Specification**: Identifies logical data types (e.g., Integer, String, Date).
- **Constraints**: Defines rules such as mandatory fields and allowable values.
- **Application Neutral**: Does not specify how the data will be physically stored or accessed.

---

### 3. Physical Data Model

#### Definition

The **Physical Data Model** translates the logical model into a specific implementation, detailing how the data will be stored in a particular database system. It includes technical details necessary for actual database construction.

#### Purpose

- Provides the specific structure required to implement the data in a chosen database management system (DBMS).
- Addresses performance, storage, and access methods, including indexing and partitioning strategies.

#### Components

- **Table Structures**: Defines how entities will be represented as tables in the database.
- **Column Specifications**: Details for each column, including data types, lengths, and constraints (e.g., NULL/NOT NULL).
- **Indexes**: Specifications for optimizing data retrieval (e.g., primary key indexes, secondary indexes).
- **Relationships and Constraints**: Implementing foreign keys, triggers, and referential integrity rules.

#### Characteristics

- **DBMS-Specific**: Tailored to the requirements and capabilities of a specific database technology.
- **Performance Considerations**: Focuses on optimizing storage and access patterns.
- **Physical Storage**: Includes specifications for physical storage, such as file organization and data distribution.

---

## Importance of Data Model Layers

- **Clarity and Structure**: Each layer provides a clear and structured approach to understanding data at different levels of abstraction, facilitating better communication and alignment among stakeholders.
- **Incremental Development**: Allows for iterative development and refinement of data models, starting from high-level concepts down to technical specifications.
- **Consistency**: Ensures that the conceptual understanding of data aligns with logical and physical implementations, reducing discrepancies and improving data integrity.
- **Scalability**: A layered approach makes it easier to scale and adapt data models to changing business needs or technologies without losing sight of the overall structure.