---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Noise and Error]]"
---

# Parity Check

**Parity checks** are basic error detection methods used to identify data transmission errors. Here’s a summary of their effectiveness and limitations:

## Simple Parity

- **Function**: Adds a parity bit to ensure an even (even parity) or odd (odd parity) number of 1s in the data.
- **Error Detection**: 
  - **Catches**: Errors that affect an odd number of bits.
  - **Does Not Catch**: Errors that affect an even number of bits or multiple bit errors.
  
## Longitudinal Parity

- **Function**: Adds parity bits for each row and column of a data block.
- **Error Detection**:
  - **Catches**: Errors in both rows and columns, improving detection compared to simple parity.
  - **Limitations**: Requires additional parity bits, leading to increased data overhead.

## Summary

- **Simple Parity**: 
  - **Strength**: Simple and requires minimal additional bits.
  - **Weakness**: Only detects errors affecting an odd number of bits; not effective for all error types.

- **Longitudinal Parity**: 
  - **Strength**: More effective at catching errors by checking both rows and columns.
  - **Weakness**: Requires more check bits, leading to increased data size and complexity.

## Need for Better Error Detection

- **Limitation**: Both simple and longitudinal parity have their limitations and may not catch all types of errors.
- **Alternative**: [[Arithmetic Checksum]] may offer a more robust method for error detection.

Understanding these methods highlights the need for more advanced error detection techniques to ensure data integrity in communication systems.
