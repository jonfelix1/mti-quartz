---
tags:
  - akpsi
  - note
Class: "[[Information System Analysis and Design Class (AKPSI)]]"
Topic: "[[Information System Project Planning and Management]]"
---

# Example Calculation: Karner's Use Case Point Estimation

### Project Details
- **Use cases**: 3 use cases
  - **Simple**: 2 transactions (Weight = 5)
  - **Average**: 5 transactions (Weight = 10)
  - **Complex**: 9 transactions (Weight = 15)
  
- **Actors**: 3 actors
  - **Simple** (Weight = 1)
  - **Average** (Weight = 2)
  - **Complex** (Weight = 3)

---

## Step 1: Calculate Unadjusted Use Case Points (UUCP)

### Use Case Weighting
- **Simple**: 1 use case × 5 = 5 points
- **Average**: 1 use case × 10 = 10 points
- **Complex**: 1 use case × 15 = 15 points

**Total Use Case Points**: $5 + 10 + 15 = 30$ points

### Actor Weighting
- **Simple**: 1 actor × 1 = 1 point
- **Average**: 1 actor × 2 = 2 points
- **Complex**: 1 actor × 3 = 3 points

**Total Actor Points**: $1 + 2 + 3 = 6$ points

### Total Unadjusted Use Case Points (UUCP)
$$
UUCP = 30 + 6 = 36 \text{ points}
$$

---

## Step 2: Calculate [[Technical Complexity Factors (TCF)]]

### 13 Technical Factors
For simplicity, assume the ratings for the 13 technical factors sum to **25**.

$$

TCF = 0.6 + (0.01 \times 25) = 0.6 + 0.25 = 0.85
$$


---

## Step 3: Calculate [[Environmental Complexity Factors (ECF)]]

### 8 Environmental Factors
Assume the ratings for the 8 environmental factors sum to **12**.

$$

ECF = 1.4 + (-0.03 \times 12) = 1.4 - 0.36 = 1.04
$$


---

## Step 4: Calculate Adjusted Use Case Points (AUCP)

$$

AUCP = UUCP \times TCF \times ECF
$$

$$

AUCP = 36 \times 0.85 \times 1.04 = 31.824 \approx 31.8 \text{ points}
$$


---

## Step 5: Estimate Effort

Assuming **20 person-hours per UCP**, the total effort estimate is:

$$

31.8 \times 20 = 636 \text{ person-hours}
$$


---

### Summary of Effort Estimation

- **Unadjusted Use Case Points (UUCP)**: 36 points
- **Adjusted Use Case Points (AUCP)**: 31.8 points
- **Effort estimate**: 636 person-hours

---

This example demonstrates how **Karner's Use Case Point Estimation** can be used to estimate effort for a software project based on use cases, technical complexity, and environmental factors.