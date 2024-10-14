---
tags:
- mandat
- note
- topic
Class: "[[Data Management Class (ManDat)]]"
---

# Structural Constraints

## Multiplicity

Multiplicity refers to the set of rules that define how entities in one entity type can relate to entities in another. It consists of two elements:

- **Cardinality**: The maximum number of times an entity can participate in a relationship.
- **Participation**: Determines whether participation in a relationship is **mandatory** or **optional**.

> Multiplicity
> ![[Pasted image 20241015011835.png#invert_B]]

## Common Degrees of Relationships

- **One-to-One (1:1)**: Each instance in one entity relates to only one instance in another.
- **One-to-Many (1:*)**: One entity instance relates to many instances in another entity.
- **Many-to-Many (_:_)**: Multiple instances of one entity can relate to multiple instances of another.

Examples:

- Staff manages Branch (1:1)
- Staff oversees PropertyForRent (1:\*)
- Newspaper advertises PropertyForRent (\*:\*)

> One to One relationship
> ![[Pasted image 20241015011932.png#invert_B]]

> One to Many Relationship
> ![[Pasted image 20241015011947.png#invert_B]]

> Many to Many Relationship
> ![[Pasted image 20241015012017.png#invert_B]]

> Multiplicity as cardinality and participation constraints
> ![[Pasted image 20241015012112.png#invert_B]]