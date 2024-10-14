---
tags:
- mandat
- note
- topic
Class: "[[Data Management Class (ManDat)]]"
---

# Database Modeling and Design

## Relational Database Design Methodology

Relational database design is a structured methodology for transforming real-world data requirements into a conceptual and then physical database model. The design process typically follows a step-by-step approach to ensure the integrity, accuracy, and efficiency of the database system.

### 1. Conceptual Database Design

Conceptual design focuses on the high-level structure of the data, independent of how it will be physically stored. The conceptual model outlines entities, their attributes, relationships, and business rules.

#### 1.1 Identify Entity Types

Entity types represent distinct objects or concepts in the domain that have an independent existence. Examples of **entity types** include **Staff**, **Customer**, **Product**, and **Sale**.

#### 1.2 Identify Relationship Types

Relationship types represent the meaningful associations between entity types. A relationship can have different degrees based on the number of entities involved:

- **Unary relationship**: A single entity type is involved in the relationship (e.g., a manager manages other employees).
- **Binary relationship**: Two entity types are involved (e.g., **Staff** manages **Branch**).
- **Ternary relationship**: Three entities participate (e.g., **Customer** buys **Product** from a **Supplier**).

#### 1.3 Identify and Associate Attributes with Entity or Relationship Types

Attributes define the characteristics of an entity or relationship. For example, a **Staff** entity could have attributes like **StaffID**, **Name**, and **DateOfHire**.

#### 1.4 Determine Attribute Domain

The attribute domain defines the set of valid values that an attribute can hold. For example, the domain for an attribute **DateOfHire** would be a **date** format.

#### 1.5 Determine Candidate, Primary, and Alternate Keys

- **Candidate Key**: A minimal set of attributes that can uniquely identify each entity occurrence.
- **Primary Key**: The selected candidate key that will uniquely identify each record in a table.
- **Alternate Key**: Other candidate keys that can be used as unique identifiers but are not the primary key.

#### 1.6 Consider Use of Enhanced Modeling Concepts

Enhanced ER modeling concepts like **generalization** and **specialization** can help model complex data relationships, such as hierarchical relationships between different entity types.

#### 1.7 Check Model for Redundancy

Identify and eliminate any redundant entities, attributes, or relationships to ensure that the data model remains efficient and free from unnecessary duplication.

#### 1.8 Validate Conceptual Data Model Against User Transactions

Ensure the model accurately supports the business processes and user transactions. This step involves validating whether the model can handle all required transactions like **create**, **read**, **update**, and **delete** operations.

#### 1.9 Review Conceptual Data Model with Users

Collaborate with stakeholders to verify that the conceptual model accurately reflects business requirements before proceeding to logical and physical design phases.

## Concepts of the ER Model

The **Entity-Relationship (ER) model** is fundamental for designing a database, providing a clear visualization of the data structure.

> 5W + 1H of ER Model
> ![[Pasted image 20241015010942.png#invert_B]]


> Has Relationship
> ![[Pasted image 20241015011122.png#invert_B]]

- [[Entity Types]]: Defines the classification of real-world objects with independent existence, such as **Staff**, **Customer**, or **Product**.
- [[Relationship Types]]: Describes associations between entity types, like **Unary**, **Binary**, or **Ternary** relationships.
- [[Attributes]]: Represents the properties of an entity or relationship, such as **Simple**, **Composite**, **Multi-valued**, or **Derived** attributes.
- [[Keys]]: Identifies unique instances of entities, including **Candidate**, **Primary**, and **Composite** keys.
- [[Structural Constraints]]: Defines the cardinality and participation rules for relationships between entities, such as **one-to-one (1:1)** or **many-to-many (_:_)**.
- [[Enhanced Entity-Relationship (EER) Model]]: Extends the basic ER model with advanced features like **specialization** and **generalization** to handle more complex applications.
- [[Database Design Methodology]]: Provides a step-by-step approach for designing relational databases, including logical and physical design processes.
- [[Domain]]: Specifies the set of valid values that can be assigned to an attribute, such as **data types**, **ranges**, and **rule-based constraints**.