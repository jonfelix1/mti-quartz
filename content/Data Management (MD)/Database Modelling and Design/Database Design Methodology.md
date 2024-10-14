---
tags:
- mandat
- note
- topic
Class: "[[Data Management Class (ManDat)]]"
---

# Database Design Methodology

## Logical Database Design for the Relational Model

### Building the Logical Data Model

- **Step 2.1: Derive Relations for Logical Data Model**
  - **Strong Entity Types**: For each strong entity, create a relation that includes all simple attributes. For composite attributes, include only the constituent simple attributes.
  - **Weak Entity Types**: Create a relation that includes all simple attributes of the weak entity. The primary key of a weak entity is derived from the owner entity.
  - **One-to-Many (1:*) Relationships**: Designate the entity on the "one" side as the parent, and the entity on the "many" side as the child. Post a copy of the parent's primary key into the child's relation as a foreign key.
  - **One-to-One (1:1) Relationships**: Handle based on participation constraints:
    - **Mandatory participation on both sides**: Combine entities into one relation and choose one primary key.
    - **Mandatory on one side**: Post the parent's primary key into the child relation.
    - **Optional on both sides**: The designation of parent and child is arbitrary unless additional information is provided.
  - **Recursive 1:1 Relationships**: Similar rules apply as for 1:1 relationships. Use two copies of the primary key or create a new relation for the recursive relationship.
  - **Superclass/Subclass Relationships**: Identify the superclass as the parent and subclass as the child. Representation options include:
    - **Option A**: Multiple relations—one for the superclass and one for each subclass.
    - **Option B**: Subclass relations only.
    - **Option C**: Single relation with a type attribute.
    - **Option D**: Single relation with multiple type attributes.
  - **Many-to-Many (*:*) Relationships**: Create a relation for the relationship, including a copy of the primary keys from the participating entities as foreign keys, which may also form the primary key of the new relation.
  - **Multi-Valued Attributes**: Create a new relation for the multi-valued attribute, including the primary key of the entity as a foreign key.

## Mapping from ER Diagram to Relations

### Key Guidelines
> Guideline for representation of superclass / subclass relationship
> ![[Pasted image 20241015013137.png#invert_B]]

- **Strong Entities**: Include all simple attributes.
- **Weak Entities**: Primary key derived from owner entity.
- **Binary Relationships**: 
  - **1:* relationships**: Parent’s primary key is added to the child’s relation.
  - **1:1 relationships**: Participation constraints determine how entities are combined or related.
- **Recursive Relationships**: Similar handling to binary relationships, using multiple copies of the primary key if needed.
- **Superclass/Subclass**: Choose from multiple options based on participation and disjointness constraints.
- **Multi-Valued Attributes**: Create new relations with primary keys of the entity as foreign keys.

### Common Scenarios
- **Many-to-Many Relationships**: A new relation is created with foreign keys from both participating entities.
- **Recursive Relationships**: Managed through additional relations or multiple primary keys depending on the participation.

> Conceptual data model for Staff view showing all attributes
> ![[Pasted image 20241015013154.png#invert_B]]