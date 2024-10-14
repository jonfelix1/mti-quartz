---
tags:
- akpsi
- note
topic: "[[Behavioural Modelling]]"
class: "[[Information System Analysis and Design Class (AKPSI)]]" 
---

# CRUDE Analysis

**CRUDE Analysis** is a technique used in object-oriented design to evaluate and clarify the interactions among classes in a system. It focuses on identifying the types of interactions (Create, Read, Update, Delete, Execute) between objects and is particularly useful in validating the behavior of a system by ensuring that all necessary interactions are accounted for.

---

## Key Components

1. **CRUDE Matrix**
   - A table format that represents the interactions between different classes or objects.
   - Each cell in the matrix indicates the type of interaction between a class (row) and an actor or another class (column).
   - The matrix is populated with letters representing the types of interactions:
     - **C**: Create
     - **R**: Read (or Reference)
     - **U**: Update
     - **D**: Delete
     - **E**: Execute

2. **Types of Interactions**
   - **Create (C)**: Indicates that one object can instantiate another object. For example, a `Patient` class can create a `MedicalRecord` object.
   - **Read (R)**: Signifies that one object can read or reference the attributes of another object. For example, a `Doctor` can read a `Patient's` details.
   - **Update (U)**: Refers to one object modifying the attributes of another object. For instance, a `Nurse` can update the `Patient's` status.
   - **Delete (D)**: Indicates that one object can remove another object. For example, a `Record` can be deleted from a `Patient's` file.
   - **Execute (E)**: Signifies that one object can call or execute methods of another object, such as a `Controller` executing a `Service` method.

---

## Steps for Conducting CRUDE Analysis

1. **Identify Classes and Actors**
   - Begin by listing all relevant classes and actors within the system.
   - Clearly define the responsibilities and roles of each class or actor.

2. **Create the CRUDE Matrix**
   - Establish a matrix with classes and actors along the rows and columns.
   - Each cell corresponds to the interaction between the entities.

3. **Populate the Matrix**
   - Analyze the interactions and fill in the matrix with the appropriate CRUDE letters (C, R, U, D, E).
   - Ensure that all possible interactions are considered.

4. **Validation and Review**
   - Review the completed matrix to ensure that it accurately reflects the interactions in the system.
   - Validate that each class can be instantiated and that the matrix does not contain any inconsistencies.

---

## Benefits of CRUDE Analysis

- **Clarifies Interactions**: It helps clarify how objects interact within the system, which can aid in identifying potential design flaws.
- **Supports Object-Oriented Design**: By focusing on object interactions, CRUDE analysis aligns with object-oriented principles and encourages collaboration among classes.
- **Facilitates Communication**: It provides a visual representation of interactions that can be easily communicated among stakeholders, including developers, analysts, and clients.
- **Identifies Complex Objects**: The frequency of Create, Update, and Delete interactions can indicate which classes might require a more complex lifecycle, potentially necessitating state modeling.
- **Guides Further Design**: It can lead to the identification of additional requirements or the need for adjustments in use cases, sequence diagrams, and other modeling elements.

---

## Example of a CRUDE Matrix

| Class/Actor  | Patient | MedicalRecord | Doctor | Nurse |
|--------------|---------|---------------|--------|-------|
| **Patient**  |    C    |       R       |   U    |   D   |
| **Doctor**   |    R    |       R       |   E    |       |
| **Nurse**    |    R    |       U       |        |   E   |

### Interpretation of the Matrix

- The **Patient** can create a `MedicalRecord`, read it, update their information, and delete records.
- The **Doctor** can read patient details and medical records, and execute methods but cannot create or delete records.
- The **Nurse** can read patient information, update records, and execute methods on related services.

---

## Conclusion

CRUDE Analysis is a valuable tool in object-oriented design that enhances the understanding of how classes and actors interact. By providing a structured approach to evaluating interactions, it ensures that the system design is robust and meets the required specifications.
