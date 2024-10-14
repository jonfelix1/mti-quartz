---
tags:
- mandat
- note
Topic: "[[Data Modelling and Design]]"
Class: "[[Data Management Class (ManDat)]]"
---

# Database Development Lifecycle

The **Database Development Lifecycle (DDLC)** is a structured approach that guides the development of a database system from initial planning to operational maintenance. This lifecycle consists of several stages, each critical for ensuring that the database meets organizational needs effectively and efficiently.

## Stages of the Database System Development Lifecycle

> The stages
> ![[Pasted image 20241015020231.png#invert_B]]

### 1. Database Planning

#### Overview
- **Purpose**: To ensure that the stages of database development are realized efficiently and effectively.
- **Integration**: Must align with the overall Information Systems (IS) strategy of the organization.

#### Key Activities
- **Identification of Enterprise Plans**: Understanding organizational goals.
- **Evaluation of Current IS**: Assessing existing systems to identify opportunities for improvement.
- **Development of Standards**: Establishing guidelines for data collection, formatting, documentation, and design.

### 2. System Definition

#### Overview
- **Scope and Boundaries**: Defines what the database will encompass and identifies major user views.

> Representation of a Database System with Multiple User Views
> ![[Pasted image 20241015020318.png#invert_B]]

#### Key Activities
- **User Views Identification**: Understanding requirements from different job roles or application areas (e.g., marketing, personnel).
- **Complexity Management**: Breaking down requirements into manageable pieces to facilitate development.

### 3. Requirements Collection and Analysis

#### Overview
- **Process**: Collecting and analyzing information about the organization to identify user requirements.

> Centralized Approach to Managing Multiple User Views
> ![[Pasted image 20241015020424.png#invert_B]]

> View Integration Approach to Managing Multiple User Views
> ![[Pasted image 20241015020448.png#invert_B]]

#### Key Activities
- **Data Description**: Documenting what data is used or generated.
- **Usage Analysis**: Understanding how data will be utilized.
- **Requirements Structuring**: Utilizing tools like Data Flow Diagrams (DFDs) or UML to organize information.

#### Approaches
- **Centralized Approach**: Merging requirements from all user views into a single set.
- **View Integration Approach**: Keeping requirements separate for each user view before merging them later.


### 4. Database Design

Database design is divided into three key phases:

#### Conceptual Database Design
- Constructs a model independent of physical considerations, focusing on high-level entities and relationships based on user requirements.

#### Logical Database Design
- Refines the conceptual model into a detailed representation based on a specific data model (e.g., relational), ensuring it remains independent of physical storage considerations.

#### Physical Database Design
- Describes how data will be stored on physical storage devices, detailing base relations, file organizations, indexes, integrity constraints, and security measures tailored to a specific DBMS.

### 5. DBMS Selection

#### Overview
- Involves choosing an appropriate Database Management System to support the database system.

#### Key Activities
- **Define Terms of Reference**: Establishing criteria for selection.
- **Shortlisting Products**: Evaluating potential DBMS options based on system requirements.
- **Recommendation and Reporting**: Producing a report on the selected DBMS.

### 6. Application Design

Application design runs parallel to database design and includes:

#### Transaction Design
- Defining characteristics of transactions required by users, including data usage, functional characteristics, outputs, and expected usage rates.

#### User Interface Design
- Creating intuitive interfaces that facilitate user interaction with the database.

### 7. Prototyping

Prototyping involves building a working model of the database system to:

- Identify features that work well or need improvement.
- Clarify user requirements.
- Evaluate feasibility of specific designs.

### 8. Implementation

This phase involves the physical realization of both database and application designs using Data Definition Language (DDL) for schema creation and Data Manipulation Language (DML) for application programming.

### 9. Data Conversion and Loading

This step transfers existing data into the new database system and may involve converting applications to function with the new setup. It is particularly relevant when replacing an older system.

### 10. Testing

Testing aims to identify errors in the database system through planned strategies using realistic data. It ensures that both the database and application programs meet specified requirements. Usability testing is also conducted against predefined criteria such as learnability and performance.

### 11. Operational Maintenance

Post-installation maintenance involves:

- Monitoring system performance.
- Tuning or reorganizing the database as necessary.
- Upgrading applications to incorporate new requirements.
