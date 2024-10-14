---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Noise and Error]]"
---

# Longitudinal Parity Check

A **longitudinal parity check** involves adding an additional parity bit for each column of data in a data block, in addition to the standard parity bit for the entire data block. This helps detect errors that may affect multiple bits in the same column.

Here is an example table illustrating longitudinal parity checks for a 4x4 data block:

| Data Bits   | Parity Bits (Row) | Parity Bits (Column) |
|-------------|-------------------|----------------------|
| 1 0 1 0     | 0                 | 0                    |
| 1 1 0 0     | 0                 | 0                    |
| 0 1 1 1     | 0                 | 0                    |
| 0 0 0 1     | 1                 | 1                    |
| **Row Parity** | 0 0 0 1         |                      |
| **Column Parity** | 1 1 1 0       |                      |

## Explanation

1. **Data Bits**: Original data arranged in a 4x4 matrix.
2. **Parity Bits (Row)**: Parity bits calculated for each row to ensure an even number of 1s.
   - Row 1: `1 0 1 0` has 2 ones (even), so parity bit = `0`.
   - Row 2: `1 1 0 0` has 2 ones (even), so parity bit = `0`.
   - Row 3: `0 1 1 1` has 3 ones (odd), so parity bit = `0` (to maintain even parity in the column).
   - Row 4: `0 0 0 1` has 1 one (odd), so parity bit = `1`.

3. **Parity Bits (Column)**: Parity bits calculated for each column to ensure an even number of 1s.
   - Column 1: `1 1 0 0` has 2 ones (even), so parity bit = `0`.
   - Column 2: `0 1 1 0` has 2 ones (even), so parity bit = `0`.
   - Column 3: `1 0 1 0` has 2 ones (even), so parity bit = `0`.
   - Column 4: `0 0 1 1` has 2 ones (even), so parity bit = `1`.

**Summary**:

- **Row Parity**: Ensures each row has an even number of 1s.
- **Column Parity**: Ensures each column has an even number of 1s.

By including both row and column parity bits, longitudinal parity checks help in detecting and correcting errors that may affect multiple bits in the same column or row, providing a more robust error detection mechanism.
