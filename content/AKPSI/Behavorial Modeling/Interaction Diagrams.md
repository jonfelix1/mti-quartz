---
tags:
- akpsi
- note
topic: "[[Behavioural Modelling]]"
class: "[[Information System Analysis and Design Class (AKPSI)]]" 
---

# Interaction Diagrams

**Interaction diagrams** are a type of **behavioural diagram** in Unified Modelling Language (UML) that model the dynamic aspects of a system. They illustrate how objects interact in a specific scenario, emphasizing the messages exchanged between them.

## Types of Interaction Diagrams

1. [[Sequence Diagram]]
    
    - **Definition**: Sequence diagrams depict how objects interact in a time-ordered sequence. They focus on the messages exchanged and the order in which they occur.
    - **Key Components**:
        - **Lifelines**: Represent the participants in the interaction, usually objects or actors.
        - **Messages**: Indicate communication between lifelines, represented as arrows between them.
        - **Activation Boxes**: Show when an object is active or controlling the flow of messages.
    - **Usage**: Suitable for modelling real-time systems and understanding the detailed flow of events in complex use cases.
2. [[Communication Diagram]]
    
    - **Definition**: Communication diagrams focus on the flow of messages between objects rather than the timing of those messages. They emphasize the structural organization of the objects involved.
    - **Key Components**:
        - **Objects and Actors**: Represent the participants in the interaction.
        - **Messages**: Indicate communication with sequence numbers to show the order.
        - **Links**: Connect objects and indicate their associations.
    - **Usage**: Useful for illustrating how objects collaborate in a more visual way, providing an overview of the message flow.

## Key Characteristics of Interaction Diagrams

- **Focus on Collaboration**: Interaction diagrams highlight how objects work together to perform a task, making them useful for understanding system behaviour.
- **Dynamic Modelling**: They provide a dynamic view of the system, showing interactions over time rather than the static structure of classes or components.
- **Use Cases Representation**: Both types of interaction diagrams can be derived from use cases, demonstrating how various scenarios unfold during system operation.

## Benefits of Interaction Diagrams

- **Clarity**: They help clarify complex interactions among objects, making it easier to understand system functionality.
- **Documentation**: Serve as effective documentation for developers and stakeholders, illustrating the behaviour of the system.
- **Communication Tool**: Facilitate communication among team members by providing a visual representation of system behaviour.

### When to Use Interaction Diagrams

- To model specific scenarios within use cases.
- When the sequence of messages and interactions is critical to understanding system behaviour.
- When presenting the dynamic aspects of a system to stakeholders or team members for analysis or review.
