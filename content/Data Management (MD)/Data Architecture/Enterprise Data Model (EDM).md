---
tags:
- mandat
- topic
- note
Class: "[[Data Management Class (ManDat)]]"
Topic: "[[Data Architecture]]"
---

# Enterprise Data Model (EDM)

The **Enterprise Data Model (EDM)** is a comprehensive, high-level representation of an organization’s data architecture. It covers all major subject areas, data entities, and the relationships between them across the entire enterprise. The EDM serves as a **blueprint** for understanding how data is used and managed within an organization, providing a unified view of the data landscape.

## Purpose of the Enterprise Data Model
- **Holistic View of Data**: The EDM helps an organization get a unified view of its data, ensuring that all stakeholders understand how data is structured and related across different departments.
- **Data Governance**: It supports data governance by helping define data stewardship roles, policies, and responsibilities for different entities.
- **Data Consistency**: By standardizing data definitions, the EDM ensures consistency in how data is defined and used across various systems and processes.
- **Decision Support**: EDM provides a strategic foundation for data-driven decision-making by ensuring that the right data is captured, structured, and made available across the organization.
- **Facilitating Integration**: It makes it easier to integrate data from different systems, ensuring that data across the organization can be seamlessly shared and analyzed.

## Components of the EDM
The Enterprise Data Model typically consists of the following key components:

---

### 1. Subject Areas
Subject areas represent major data domains that are critical to the business. Examples of subject areas include:
- **Customer**
- **Product**
- **Order**
- **Inventory**
- **Sales**
- **Finance**

Each subject area focuses on a different business function or concept and organizes the data entities accordingly.

---

### 2. Business Entities
Business entities are the core objects that represent the key objects within each subject area. These entities are typically nouns that represent tangible or intangible things of importance to the business.

- **Customer**: Represents the people or organizations that buy products.
- **Product**: Represents items or services that the organization sells.
- **Order**: Represents a customer’s request for one or more products.
- **Employee**: Represents workers or staff within the organization.
- **Invoice**: Represents the document sent to the customer for payment.

Each entity has attributes and relationships with other entities within the EDM.

---

### 3. Entity Relationships
The relationships between business entities define how they are connected to one another. These are represented using **entity-relationship diagrams (ERD)** that indicate the cardinality (one-to-many, many-to-many, etc.).

- Example: **Customer** places **Order** (one-to-many relationship).
- Example: **Order** contains **Product** (many-to-many relationship).

Relationships are essential for understanding how data flows through different business processes and for identifying how different systems interact with the same entities.

---

### 4. Data Stewardship and Accountability
For each entity, the EDM defines **data stewardship** by assigning accountability for maintaining the data’s accuracy, privacy, and security. Data stewards are responsible for ensuring the integrity and quality of the data in their domain.

- Example: A **Customer Data Steward** might be responsible for defining policies on customer data, ensuring data quality, and controlling access to sensitive customer information.

---

### 5. Business Definitions and Glossary
Each entity and attribute in the EDM must have a clear and concise **business definition**. This is crucial for ensuring that everyone in the organization understands the purpose and meaning of the data.

- Example: **Customer**: "An individual or organization that purchases goods or services from the business."
- Example: **Order Date**: "The date on which the customer places the order."

Additionally, the EDM typically includes a **business glossary** that provides common terminology, synonyms, acronyms, and distinctions between closely related terms.

---

### 6. Business Identifiers and Keys
The EDM also defines **business identifiers** for each entity, specifying the unique keys that will be used to identify instances of the entity.

- Example: For the **Customer** entity, the business identifier might be **Customer ID**, which uniquely identifies each customer.
- Example: For the **Order** entity, the business identifier might be **Order Number**.

---

### 7. Data Quality Rules
The EDM includes high-level data quality rules that ensure data is valid, complete, and consistent across systems. This might include rules on:
- **Uniqueness**: Each business entity (e.g., Customer, Product) must have a unique identifier.
- **Completeness**: All mandatory attributes must be filled in (e.g., a Customer must have a Name and Address).
- **Validation**: Attribute values must adhere to predefined constraints (e.g., a valid email format for a Customer Email attribute).

---

### 8. Integration with Other Systems
The EDM serves as a guide for integrating data across different systems. It helps to identify **shared entities** between systems and how data should be mapped for seamless integration.

- For example, a customer entity might exist in both the **CRM** system and the **Order Management** system. The EDM will define how these entities are synchronized and how the data flows between the systems.

---

### 9. Version Control and Change Management
The EDM must be **dynamic** and **evolve** over time to accommodate changes in business processes, new systems, or evolving data requirements. As such, version control and change management are critical components of maintaining the EDM.

- **Version control** ensures that all changes to the data model are tracked and documented, so users always work with the latest version.
- **Change management** processes must be established to review and approve changes to the data model, ensuring they align with business needs and data governance policies.

---

## Benefits of an Enterprise Data Model
- **Improved Data Governance**: By centralizing the organization’s data, the EDM supports better data governance practices, ensuring that data is accurate, consistent, and properly managed.
- **Enhanced Decision-Making**: With a unified and consistent view of the organization’s data, decision-makers can rely on high-quality data to support business decisions.
- **Better Data Integration**: The EDM simplifies data integration efforts, making it easier to connect disparate systems and ensure that data flows seamlessly across the organization.
- **Increased Agility**: By understanding the structure and relationships of the data, the organization can quickly adapt to changes in business processes, systems, or regulatory requirements.
