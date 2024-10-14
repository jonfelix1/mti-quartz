---
tags:
  - sip
  - note
Class: "[[Enterprise System Class (SIP)]]"
Topic: "[[Enterprise System Architecture (ESA)]]"
---



# Three-Tier Architecture

>Three-Tier Architecture
>![[Pasted image 20240906195559.png#invert_B]]

- Most current **ERP implementations** follow a **three-tiered architecture** consisting of:
    - **Web tier**
    - **Application tier**
    - **Data tier**

## Web Tier

- Includes the server that clients interact with for **application access**.
    - **GUI**, inputting data, requesting information, presenting data.
    - Consider the number of **users** during peak hours and the **type of data** transmitted.
    - Implement **security measures**: **firewall**, **policy**, **access restriction**, and **intrusion detection service**.

## Application Tier

- Provides the components to apply **business logic** of the functional modules.
    - Acts as an **intermediary** between client applications and the **database**.
    - Contains **reusable objects** of business process rules.
    - Most **processing** occurs here.
    - Requires **stringent security measures**.

## Data Tier

- Responsible for **data management**.
    - Central **repository** of data.
    - Includes **SQL manager**.
    - **Scalability** for future data needs should be anticipated.
    - Requires **stringent security measures**.


