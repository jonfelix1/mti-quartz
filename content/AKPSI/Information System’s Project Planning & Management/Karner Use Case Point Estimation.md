---
tags:
  - akpsi
  - note
Class: "[[Information System Analysis and Design Class (AKPSI)]]"
Topic: "[[Information System Project Planning and Management]]"
---

# Karner Use Case Point Estimation

**Karner's Use Case Point (UCP) Estimation** is a method used to estimate the **effort** and **time** required for a software development project based on **use cases**. It is particularly useful for projects driven by **object-oriented analysis and design**.

## Key Components of Karner’s UCP Estimation

1. **Unadjusted Use Case Points (UUCP)**:
   - **Use Case Weighting**: Each use case is categorized as **simple**, **average**, or **complex** based on the number of **transactions**.
     - **Simple**: 1-3 transactions (Weight: 5)
     - **Average**: 4-7 transactions (Weight: 10)
     - **Complex**: More than 7 transactions (Weight: 15)
   - **Actor Weighting**: Each actor is also categorized by complexity:
     - **Simple** (Weight: 1)
     - **Average** (Weight: 2)
     - **Complex** (Weight: 3)

   **UUCP** = Total Use Case Points (from use cases) + Total Actor Points (from actors)

2. [[Technical Complexity Factors (TCF)]]:
   - Consists of **13 factors** that assess the project’s technical challenges (e.g., performance, security, concurrency). Each factor is assigned a value between 0 and 5, indicating the impact on the project.
   - **TCF** formula: 
     $$
     TCF = 0.6 + (0.01 \times \text{{sum of technical factor ratings}})
     $$

3. [[Environmental Complexity Factors (ECF)]]:
   - Involves **8 factors** that evaluate environmental and team factors (e.g., team experience, development tools, motivation). These factors are also rated between 0 and 5.
   - **ECF** formula:
     $$
     ECF = 1.4 + (-0.03 \times \text{{sum of environmental factor ratings}})
     $$

4. **Adjusted Use Case Points (AUCP)**:
   - After calculating the **UUCP**, it is adjusted using the **TCF** and **ECF**:
$$
   AUCP = UUCP \times TCF \times ECF
$$

5. **Effort Estimation**:
   - To estimate the total effort, the **AUCP** is multiplied by the average effort per UCP (typically between **20** and **36 person-hours** per use case point).

**Key steps in UCP estimation**:
1. **Identify use cases** and **actors**, and assign complexity weights.
2. **Calculate the UUCP**.
3. Evaluate the **TCF** and **ECF** and calculate the **AUCP**.
4. Multiply the **AUCP** by a standard value to estimate the total **effort in person-hours**.

This method provides a systematic approach to estimating project **effort** by considering both the **use case model** and the **complexity** of technical and environmental factors.

Example - [[Example Calculation - Karner Use Case Point Estimation]]
