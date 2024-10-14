---
tags:
- akpsi
- topic
- note
Class: "[[Information System Analysis and Design Class (AKPSI)]]"
Topic: "[[Business Process and Functional Modeling]]"
---

# Use Cases Description

## Overview
- The primary driver for all UML diagramming techniques.
- Depicts activities performed by the users.
- Describes basic functions of the system:
  - What the user can do.
  - How the system responds.
- Use cases are building blocks for continued design activities.
- Each use case describes **one and only one function**.
- [[Use Cases Description Examples]]

## Purpose and Information Table

| Purpose | Overview| Detail | 
|---------|-----------------------|----------|
| Essential | High-level overview of issues essential to understanding required functionality | Detailed description of issues essential to understanding required functionality |
| Real | High-level overview of a specific set of steps performed on the real system once implemented | Detailed description of a specific set of steps performed on the real system once implemented |

## Use Case Writing Guidelines
1. Write in the form of subject-verb-direct object.
2. Make sure it is clear who the initiator of the step is.
3. Write from an independent observer’s perspective.
4. Write at about the same level of abstraction.
5. Ensure the use case has a sensible set of steps.
6. Apply the **KISS** principle liberally.
7. Write repeating instructions after the set of steps to be repeated.

## Creating Use-Case Descriptions
1. Pick a high-priority use case and create an overview:
   - List the **primary actor**.
   - Determine its type (overview or detail; essential or real).
   - List all **stakeholders** and their interests.
   - Determine the level of importance of the use case.
   - Briefly describe the use case.
   - List what **triggers** the use case.
   - List its relationship to other use cases.
2. Fill in the steps of the **normal flow of events** required to complete the use case.
3. Ensure that the steps listed are not too complicated or long and are consistent in size with other steps.
4. Identify and write the **alternate or exceptional flows**.
5. Carefully review the use case description and confirm that it is correct.
6. Iterate over the entire set of steps again.

## Elements of a Use Case Description
- **Overview**:
  - Name, ID Number, Type, Primary Actor, Brief Description, Importance Level, Stakeholder(s), Trigger(s).
- **Relationships**:
  - **Association**: Communication between the use case and the actors.
  - **Extend**: Extends the functionality of a use case.
  - **Include**: Includes another use case.
  - **Generalization**: Allows use cases to support inheritance.
- **Flow of Events**:
  - **Normal flow**: The usual set of activities.
  - **Sub-flows**: Decomposed normal flows to simplify the use case.
  - **Alternate or exceptional flows**: Those not considered the norm.
  - **Optional characteristics** (complexity, time, etc.).

## Verifying & Validating a Use Case
- Use cases must be verified and validated before beginning structural and behavioral modeling.
- Utilize a **walkthrough**:
  - Perform a review of the models and diagrams created so far.
  - Performed by individuals from the development team and the client (very interactive).
- **Facilitator**: Schedule and set up the meeting.
- **Presenter**: The one responsible for the specific representation being reviewed.
- **Recorder (scribe)**: Takes notes and documents errors.

## Rules for Verification & Validation
1. Ensure one recorded event in the flows of the use case description for each action/activity on the activity diagram.
2. All objects in an activity diagram must be mentioned in an event of the use case description.
3. The sequence of the use case description should match the sequence in the activity diagram.
4. One and only one description for each use case.
5. All actors listed in a use case description must be shown on the use case diagram.
6. Stakeholders listed in the use case description may be shown on the use case diagram (check local policy).
7. All relationships in the use case description must be depicted on the use case diagram.
8. All diagram-specific rules must be enforced. 


