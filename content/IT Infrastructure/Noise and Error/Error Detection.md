---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Noise and Error]]"
---

# Error Detection

Error detection is essential for identifying issues in data transmission despite the use of prevention techniques. Here’s an overview of the fundamental methods used for detecting errors:

## Overview

- **Purpose**: Error detection involves adding additional information to data or signals to help identify errors that may occur during transmission.
- **Method**: An **error detection code** is added to the data to facilitate the identification of errors.

## Basic Techniques

### [[Parity Check]]

- **Definition**: Adds an extra bit to data to make the total number of 1s either even or odd.
- **Types**:
    - **Even Parity**: The parity bit is set so that the total number of 1s is even.
    - **Odd Parity**: The parity bit is set so that the total number of 1s is odd.
- **Detection**: Can detect single-bit errors. If the received data does not match the expected parity, an error is indicated.

### [[Arithmetic Checksum]]

- **Definition**: Adds a value derived from the data to detect errors.
- **Process**:
    - Data is divided into chunks, and the sums of these chunks are calculated.
    - The result is sent along with the data.
- **Detection**: At the receiver end, the checksum is recalculated and compared with the transmitted checksum. Mismatches indicate errors.

### [[Cyclic Redundancy Checksum (CRC)]]

- **Definition**: Uses polynomial division to detect errors in data.
- **Process**:
    - Data is treated as a polynomial and divided by a predetermined polynomial (the generator).
    - The remainder from this division is appended to the data.
- **Detection**: The receiver performs the same polynomial division. If the remainder is zero, the data is assumed to be error-free; otherwise, an error is detected.

## Summary

- **Error Detection**: Involves adding extra information to data to identify transmission errors.
- **Techniques**:
    - **Parity Checking**: Simple method to detect single-bit errors.
    - **Arithmetic Checksum**: Adds values derived from data to detect errors.
    - **Cyclic Redundancy Check (CRC)**: Uses polynomial division to detect errors with high accuracy.

These error detection methods help ensure data integrity and reliability by identifying errors that may occur during transmission and allowing for appropriate corrective actions.
