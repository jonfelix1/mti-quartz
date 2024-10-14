---
tags:
- akpsi
- note
- topic
Class: "[[Information System Analysis and Design Class (AKPSI)]]"
---

# Structural Modelling

## Objectives
- Understand the rules and **style guidelines** for creating:
  - [[CRC Card]]
  - [[Class Diagrams]]
  - [[Object Diagrams]]
- Understand the processes used to create CRC cards, class diagrams, and object diagrams.
- Be able to create CRC cards, class diagrams, and object diagrams.
- Understand the **relationship among structural models**.
- Understand the **relationship between structural and functional models**.

## Introduction
- **Functional models** represent system behavior.
- **Structural models** represent system objects and their relationships, including:
  - People
  - Places
  - Things

## Structural Models
- Drawn using an **iterative process**:
  - Initially drawn in a **conceptual, business-centric** way.
  - Refined in a **technology-centric** way describing the actual databases and files.
  - More detail is added in each iteration.
- Create a vocabulary for analysts and users.
- Has Defined Object in [[Structural Modeling Objects]]
- Facilitate effective communication between analysts and users.

## Main Goal
- Discover the key data contained in the **problem domain** and build a structural model of the objects.
- Transform the **problem domain** into the **solution domain** through structural modelling.

## 7 Steps to Create Structural Models

1. **Create CRC Cards**:
    
    - Document responsibilities and collaborations of classes.
2. **Review CRC Cards**:
    
    - Identify any missing objects, attributes, operations, or relationships.
3. **Role-play the CRC Cards**:
    
    - Simulate interactions to find breakdowns and correct issues; create new cards as needed.
4. **Create the Class Diagram**:
    
    - Visualize the classes and their relationships based on the CRC cards.
5. **Review the Class Diagram**:
    
    - Eliminate unnecessary classes, attributes, operations, or relationships to streamline the model.
6. **Incorporate Patterns**:
    
    - Utilize common design patterns to enhance the structure.
7. **Review and Validate the Model**:
    
    - Ensure the model accurately represents the intended system structure.

## Verifying & Validating the Model

- **Presentation**:
    - Analysts present the model to developers and users, explaining the reasoning behind each class.

### Rules for Verification & Validation

1. Each **CRC card** corresponds to a specific class.
2. Responsibilities on the front of the card translate into operations on the class diagram.
3. Collaborators listed on the front imply relationships documented on the back.
4. Attributes on the back of the card must appear as attributes on the class diagram.
5. Each attribute has a defined **data type** (e.g., salary as a number format).
6. Relationships must be accurately depicted, including:
    - **Aggregation/Association**
    - **Multiplicity**
7. Use **association classes** to include attributes that describe a relationship.