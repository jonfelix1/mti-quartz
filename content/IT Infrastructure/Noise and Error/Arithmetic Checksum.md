---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Noise and Error]]"
---

# Arithmetic Checksum

**Arithmetic checksum** is a method used to detect errors in data transmission by performing a numerical sum of the data and including the result with the transmission. Here's how it works:

## Overview

- **Usage**: Commonly used in protocols like TCP and IP on the Internet.
- **Process**:
  - **Conversion**: Convert characters to numeric form.
  - **Summation**: Sum the numeric values.
  - **Transmission**: Include the sum (or its manipulated form) with the data.

## Example

1. **Data**: 4 bytes with values `56`, `72`, `34`, and `48`.
2. **Summation**: Calculate the total sum:
   - \( 56 + 72 + 34 + 48 = 210 \)
3. **Manipulate Sum**: Simplify the sum to fit a specific format, e.g., 
   - \( 210 \rightarrow 2 + 10 = 12 \)
4. **Transmission**: Send the data along with the checksum value `12`.
5. **Receiver**: Performs the same summation and manipulation to verify the checksum.

## Limitations

- **Detection**: While arithmetic checksum improves error detection over simple parity, it still may not catch all errors.
- **Need for Improvement**: **Cyclic Redundancy Check (CRC)** offers a more robust error detection method.

## Summary

- **Arithmetic Checksum**: Converts data to numeric form, sums it, and includes the result with the transmission.
- **Limitations**: Not entirely foolproof; may not detect all types of errors.

**Next Step**: Explore **Cyclic Redundancy Check (CRC)** for a more reliable error detection technique.
