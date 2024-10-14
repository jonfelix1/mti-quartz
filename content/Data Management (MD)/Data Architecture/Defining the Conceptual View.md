---
tags:
- mandat
- topic
- note
Class: "[[Data Management Class (ManDat)]]"
Topic: "[[Data Architecture]]"
---

# Defining the Conceptual View

The **conceptual view** focuses on capturing the high-level structure of the business, representing the entities and their relationships without getting into specific details of the system or technical implementations. This is the first step in developing a data model.

## 1. Identify and Name Business Entities

- **Entities** represent significant business objects (e.g., Customer, Order, Product, Employee) that need to be captured in the system.
- Naming entities should align with the business's common terminology.

## 2. Identify Super-type / Sub-types

- This step involves defining any **hierarchies** or **relationships** between entities.
    - Example: _“Customer”_ could be a super-type with sub-types like _“Individual Customer”_ and _“Business Customer.”_
- Use the "X is a kind of Y" format to define these relationships.
- It is often beneficial to isolate class hierarchies into separate **subject areas** to maintain clarity in the model.

## 3. Draft, Review, and Refine Entity Business Definitions

- Write **business definitions** for each entity, explaining their role and significance in the business context. This ensures shared understanding across stakeholders.
- Review these definitions with business users and refine them based on feedback.

## 4. Identify and Specify Examples, Synonyms, Acronyms

- Identify any **alternative terms** that could refer to the same entity (synonyms, acronyms).
    - Example: _“Customer”_ might also be referred to as _“Client.”_
- Provide **examples** of entities to help stakeholders understand their meaning.

## 5. Document Distinctions from Closely Related Terms

- It is important to differentiate similar or closely related terms, ensuring that entities are not confused with one another.
    - Example: _“Order”_ vs. _“Invoice.”_

## 6. Assign Primary Subject Area

- Group entities into **subject areas** based on their relevance to different parts of the business.
    - Example: "Customer" may belong to the **Sales** subject area, while "Product" may belong to the **Merchandising** subject area.

## 7. Assign Data Stewardship Accountability

- Assign responsibility for each entity to a **data steward**. Data stewards are responsible for maintaining the accuracy, privacy, and security of data related to that entity.

## 8. Define Potential Business Identifiers

- Identify possible **business identifiers** for each entity (e.g., Customer ID, Order Number) that will be used to uniquely identify records.

## 9. Define Initial Draft Primary Key Attribute

- Propose a **primary key** for each entity. This is the attribute or combination of attributes that uniquely identifies each record in the entity.

## 10. Identify and Specify Business Relationships

- Define the **relationships** between entities.
    - Example: A "Customer" _places_ an "Order."
- Include the **cardinality** of the relationships (e.g., one-to-many, many-to-many).
