---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Noise and Error]]"
---

# Hamming Code

**Hamming Code** is an error-correcting code used to detect and correct single-bit errors in data transmission. It uses additional parity bits added to the original data bits to create a code that can identify and correct errors.

## Principles

- **Redundant Bits**: Hamming code adds redundant bits to the original data bits.
- **Error Detection and Correction**: The code can detect and correct single-bit errors.
- **Parity Bits**: Each parity bit covers a specific set of bits in the code.

## Example Calculation

Let's encode the data `1011` using a Hamming (7,4) code, which uses 4 data bits and 3 parity bits.

### Step-by-Step Encoding

1. **Determine Positions of Parity Bits**:
   - Parity bits are placed at positions that are powers of 2: 1, 2, 4.
   - Data bits are placed in the remaining positions: 3, 5, 6, 7.

   ```
   Position: 1 2 3 4 5 6 7
   Bit:      P P D P D D D
   ```

2. **Place Data Bits**:
   - Data `1011` is placed in positions 3, 5, 6, 7.

   ```
   Position: 1 2 3 4 5 6 7
   Bit:      P P 1 P 0 1 1
   ```

3. **Calculate Parity Bits**:

   - **Parity Bit 1 (P1)**: Covers bits at positions 1, 3, 5, 7.
     - `P1` should make the number of 1s in these positions even.
     - `P1` = 1 (to make the count even: 1, 1, 0, 1)

   - **Parity Bit 2 (P2)**: Covers bits at positions 2, 3, 6, 7.
     - `P2` should make the number of 1s in these positions even.
     - `P2` = 0 (to keep the count even: 0, 1, 1, 1)

   - **Parity Bit 4 (P4)**: Covers bits at positions 4, 5, 6, 7.
     - `P4` should make the number of 1s in these positions even.
     - `P4` = 1 (to make the count even: 1, 0, 1, 1)

   ```
   Position: 1 2 3 4 5 6 7
   Bit:      1 0 1 1 0 1 1
   ```

4. **Encoded Message**: The encoded Hamming code for `1011` is `1011011`.

## Error Detection and Correction

- **Received Code**: Suppose the receiver gets `1010011`.
- **Check Parity Bits**:
  - Compute parity for each position and compare with received values.
  - If there's an error, the parity check will identify the bit position with the error.
- **Correct Error**: Flip the identified bit to correct the error.

Hamming code effectively detects and corrects single-bit errors and is widely used in data communication systems.
