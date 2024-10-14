---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Making Connection Efficient]]"
---

# Differential Encoding

**Differential Encoding** is a technique used in video compression to efficiently store and transmit video data by focusing on the differences between consecutive frames. Here's an overview of how this method works:

## Principle

- **Video Compression Challenge**: Run-length encoding is not effective for video compression because frames in a video generally have little similarity in color values across the entire frame.
- **Differential Encoding**: Instead of storing each full frame, only the differences between consecutive frames are stored. This method takes advantage of the fact that neighboring frames often change only slightly.

## Process

1. **Store Initial Frame**:
   - The first frame is stored completely in a buffer.

2. **Compute Differences**:
   - For each subsequent frame, compute the difference from the previously stored frame.

3. **Store Differences**:
   - Store the computed differences rather than the full frame data.

4. **Update Buffer**:
   - Store the current frame as the new reference frame for future comparisons.

## Example

Given the following frames:

### First Frame

```
5 7 6 2 8 6 6 3 5 6
6 5 7 5 5 6 3 2 4 7
8 4 6 8 5 6 4 8 8 5
5 1 2 9 8 6 5 5 6 6
```

### Second Frame

```
5 7 6 2 8 6 6 3 5 6
6 5 7 6 5 6 3 2 3 7
8 4 6 8 5 6 4 8 8 5
5 1 3 9 8 6 5 5 7 6
```

### Difference Frame

```
0 0 0 0 0 0 0 0 0 0
0 0 0 1 0 0 0 0 -1 0
0 0 0 0 0 0 0 0 0 0
0 0 1 0 0 0 0 0 1 0
```

In this example:
- The difference frame shows how the values have changed between the first and second frames. 
- A value of `0` indicates no change, while non-zero values indicate changes.

## Advantages

- **Efficient Storage**: Only changes from frame to frame are stored, which can significantly reduce the amount of data required.
- **Lossless**: The difference encoding is typically lossless, meaning that the exact original frames can be reconstructed from the stored differences.

## Limitations

- **Temporal Dependency**: Requires that the previous frame be available to reconstruct the current frame.
- **Error Propagation**: Errors or artifacts in one frame can propagate to subsequent frames if not managed correctly.

Differential encoding is widely used in video compression formats, such as MPEG and H.264, to efficiently encode video data by focusing on the temporal redundancy between frames.
