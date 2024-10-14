---
tags:
- akpsi
- topic
- note
Class: "[[Information System Analysis and Design Class (AKPSI)]]"
Topic: "[[Business Process and Functional Modeling]]"
---

# Activity Diagram

[[Business Process and Functional Modeling]] involves representing the activities within a business process, often with **activity diagrams**.

## Key Concepts

- **Business Processes**: Consist of a series of **activities** that are performed to achieve specific business goals.
    
- **Activity Diagrams**:
    - **Depict the sequence** of activities within a process.
    - Derived from [[Use Case Diagram]]
    - Are **abstract**, meaning they describe processes generally, without focusing on specific implementation details.
    - Has a standardized [[Activity Diagram Symbols]]
    - **Model behavior independently** of the objects or systems involved.
    - Can be applied to model **any type of process**, whether business-related or not.

These diagrams help in understanding and optimizing workflows by visually representing how tasks flow through a process.

---

## Guidelines for Activity Diagrams

### 1. Set the Scope of the Activity Being Modeled
- Clearly define the **boundaries** of the process.
- Understand the **start** and **end points** of the activity being diagrammed.

### 2. Identify the Activities and Connect Them with Flows
- Break down the business process into distinct **activities** or tasks.
- Use **arrows** to connect activities, showing the flow of control.

### 3. Identify Any Decisions That Must Be Made
- Highlight decision points where a choice is needed using **decision nodes** (diamond shape).
- Define the **outcomes** for each decision to show different paths.

### 4. Identify Potential Parallelism in the Process
- Look for activities that can happen **simultaneously**.
- Use **fork** and **join nodes** to represent **parallel processes**.

### 5. Draw the Activity Diagram
- Create the final diagram, ensuring that the flow of activities is clear.
- Use symbols like **action nodes**, **start/end nodes**, **fork/join nodes**, and **decision/merge nodes**.

---

## Creating an Activity Diagram

### 1. Choose a Business Process Identified Previously
- Select a business process to model, based on the **use-case** and **requirements definition**.

### 2. Review the Requirements Definition and Use-Case Diagram
- Ensure the activities align with the documented **requirements** and **use-cases**.

### 3. Review Other Documentation Collected
- Look through existing documentation to identify any **additional details** or processes involved.

### 4. Identify the Set of Activities Used in the Business Process
- List all the specific **actions or tasks** in the process.

### 5. Identify Control Flows and Nodes
- Define how the process **flows** between activities and any **decisions** or **branching points**.

### 6. Identify Object Flows and Nodes
- Determine the movement of **objects** (data or materials) between activities.

### 7. Lay Out & Draw the Diagram
- Sketch the diagram, ensuring **clarity** and **minimal crossing lines** for better understanding.