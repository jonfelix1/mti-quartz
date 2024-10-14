---
tags:
  - akpsi
  - note
Class: "[[Information System Analysis and Design Class (AKPSI)]]"
Topic: "[[Structural Modelling]]"
---

# CRC Cards
- **Class-responsibility-collaboration** card

## Overview
- **Index cards** used to document the responsibilities and collaborations of a class.

## Responsibilities
- **Knowing**:
  - What a class must know, manifested as **attributes**.
- **Doing**:
  - What a class must do, manifested later as **operations**.

## Collaboration
- Involves objects working together to service a request:
  - **Requestor (client)**: The object making the request.
  - **Responder (server)**: The object fulfilling the request.
  - Bound by a **contract**.

## CRC Cards & Role-Playing
- An exercise to help discover additional objects, attributes, relationships, and operations:
  - Team members perform roles associated with the actors and objects previously identified.
  - Utilize activity diagrams to run through the steps in a scenario.
  - Identify an important use-case and assign roles based on actors and objects.
  - Team members perform each step in the scenario.
  - Discover and fix problems until a successful conclusion is reached.
  - Repeat for remaining use-cases.

---

## Example of a CRC Card

### CRC Card for a Library Book Class

| Class: **LibraryBook** |
|-------------------------|
| **Responsibilities**    |
| **Knowing:**            |
| - Title                 |
| - Author                |
| - ISBN                  |
| - Availability Status    |
| **Doing:**              |
| - CheckOut()            |
| - CheckIn()             |
| - Reserve()             |
| - GetDetails()          |
| **Collaborators**       |
| - User (Requestor)      |
| - LibrarySystem (Responder) |

### Explanation
- **Class Name**: Indicates the class being documented, in this case, **LibraryBook**.
- **Responsibilities**:
  - **Knowing**: Lists attributes that the class must maintain, like title, author, ISBN, and availability status.
  - **Doing**: Lists operations that the class can perform, such as checking out and checking in the book, reserving it, and getting its details.
- **Collaborators**: Identifies the objects that the class interacts with, including the **User** (requestor) and the **LibrarySystem** (responder).

