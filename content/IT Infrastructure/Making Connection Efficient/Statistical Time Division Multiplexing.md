---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Making Connection Efficient]]"
---

# Statistical Time Division Multiplexing (STDM)

- A **statistical multiplexor** transmits data only from **active workstations**.
- If a workstation is not active, no space is wasted in the **multiplexed stream**.

## Frame Creation
- The multiplexor creates a **frame** containing data from active workstations.
- Each piece of data includes an **address** for identification.
- If data size varies, the **length** of the data must also be included.

>If the data is of variable size, a length is also included
![[Pasted image 20240912193212.png#invert_B]]


>A more complete picture
![[Pasted image 20240912193234.png#invert_B]]
