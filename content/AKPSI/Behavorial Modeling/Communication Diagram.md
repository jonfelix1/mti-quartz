---
tags:
- akpsi
- note
topic: "[[Behavioural Modelling]]"
class: "[[Information System Analysis and Design Class (AKPSI)]]" 
---

# Communication Diagram

A **communication diagram** is a type of interaction diagram in **Unified Modelling Language (UML)** that illustrates how objects interact within a system through messages. It emphasizes the structural organization of the objects that interact and the messages exchanged among them, rather than the time sequence of these interactions.

> Communication Diagram
> ![[Pasted image 20241009195122.png#invert_B]]

## Key Components of Communication Diagrams

1. **Objects and Actors**
   - Represented as labelled rectangles or ovals, indicating the participants in the interaction.
   - Each object or actor is connected through lines to demonstrate their relationships.

2. **Links**
   - Solid lines connecting the objects represent associations or links.
   - Links indicate which objects can communicate with each other.

3. **Messages**
   - Labelled arrows on the links denote messages sent from one object to another.
   - Each message is numbered to indicate the sequence of interaction (e.g., 1, 2, 3).
   - Optional parameters can be included in parentheses next to the message name.

4. **Sequence Numbers**
   - Messages are numbered to show the order of interactions, facilitating an understanding of the communication flow.
   - The numbering system indicates the sequence in which messages are exchanged.

## Syntax of Communication Diagrams

- Objects: Represented as boxes labelled with the object’s name and class.
- Links: Solid lines connecting the objects represent associations.
- Messages: Labelled arrows along the links, with optional parameters in parentheses.
- Sequence Numbers: Indicate the order of messages.

## Purpose and Usage

- **Modelling Use Cases**: Communication diagrams help model the interactions defined in use cases, providing insights into how objects collaborate to achieve specific functionality.
- **Highlighting Structure**: They emphasize the structural relationships between objects, showcasing how they are interconnected within the system.
- **Facilitating Understanding**: Useful for visualizing complex interactions in a more compact form compared to sequence diagrams.

## Benefits of Communication Diagrams

- **Clarity**: Provide a clear representation of the relationships among objects and the messages exchanged, making them easier to understand for stakeholders.
- **Compactness**: More concise than sequence diagrams, allowing for a quicker grasp of object interactions without the temporal emphasis.
- **Complementary Tool**: Can be used alongside sequence diagrams to provide different perspectives on the same interactions.
