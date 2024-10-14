---
tags:
- mandat
- note
- topic
Class: "[[Data Management Class (ManDat)]]"
---

# Domain

**Domain** refers to the complete set of possible values that can be assigned to an attribute. It standardizes the characteristics of attributes within a logical or physical data model.

For instance, a **Date domain** includes all valid date values and can be used for date-related attributes, such as **EmployeeHireDate**, **OrderEntryDate**, **ClaimSubmitDate**, or **CourseStartDate**.

## Types of Domains

- **Data Type Domain**: Specifies the standard types of data an attribute can have, such as:
  - **Integer**
  - **Character(30)**
  - **Date**

- **Data Format Domain**: Uses patterns or templates to define valid values. This can include:
  - **Postal codes**
  - **Phone numbers**
  - **Character limitations** (e.g., alphanumeric, special characters)

- **List Domain**: Contains a finite set of predefined values, similar to dropdown lists. For example:
  - **OrderStatusCode** can be restricted to values like **Open**, **Shipped**, **Closed**, **Returned**.

- **Range Domain**: Specifies a range of acceptable values for a data type, which can be open-ended. For example:
  - **OrderDeliveryDate** must be between **OrderDate** and three months in the future.

- **Rule-based Domain**: Defined by rules that ensure the validity of values by comparing them to calculated values or other attributes. For example:
  - **ItemPrice** must be greater than **ItemCost**.

Domains provide a structured way to ensure consistency and integrity across data models by restricting the values that can be assigned to specific attributes.