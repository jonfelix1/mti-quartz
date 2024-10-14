---
tags:
- mandat
- topic
- note
Class: "[[Data Management Class (ManDat)]]"
Topic: "[[Data Architecture]]"
---

# Defining the Logical View

The **logical view** provides a more detailed data structure, describing the essential data attributes and their relationships in a way that remains **application-neutral**. It is still abstract, focusing on what data is required rather than how it will be implemented.

## 1. Still Usage (Application) Neutral

- The logical data model is still independent of any specific application, representing data requirements rather than the system that will manage it.

## 2. Identify Essential Data Attributes

- For each entity, identify its **key attributes** (data fields) such as **unique identifiers** (e.g., Order ID, Product Code), descriptive data (e.g., Customer Name, Product Description), and other relevant fields.
    - **Brainstorm by data type**: Consider different types of data like names, codes, dates, and measures that may be associated with the entity.
    - **Analyze existing data models**: Look at existing databases, forms, and reports for insights.
    - Avoid accepting the current system's data model without question, as it may not reflect actual business needs.

## 3. Assign to Logical Data Types (Domains)

- Assign each attribute to a **logical data type** (e.g., string, date, number). Logical data types describe the kind of data each field will store without defining specific implementation (e.g., VARCHAR, INTEGER).
    - Inherit **standard length** for the domain if applicable.
    - Example: Names might be strings with a length of 100 characters, while dates are formatted as `YYYY-MM-DD`.

## 4. Name According to Standards

- Attribute names should follow **naming conventions** that are agreed upon by the organization. Names should be meaningful and consistent across the model.

## 5. Draft, Review, and Refine Attribute Definitions

- Define the purpose and meaning of each attribute, ensuring it’s clear to both technical and non-technical users.
    - Example: _Customer Name_ - "The full name of the customer making the purchase."

## 6. Determine Null-ability

- Decide whether an attribute can have a **null** value. Some fields, like a primary key, must be mandatory, while others may be optional.
    - Example: A customer’s **email address** may be optional, while their **ID** must be mandatory.

## 7. Identify Best (if any) Default Value

- For attributes that are optional or frequently left blank, determine the best **default value** (if any).
    - Example: For an optional **Customer Discount Rate** field, a default of "0%" could be assigned when the field is left blank.