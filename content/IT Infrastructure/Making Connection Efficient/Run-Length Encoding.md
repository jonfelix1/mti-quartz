---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Making Connection Efficient]]"
---

# Run-Length Encoding

**Run-Length Encoding (RLE)** is a simple and effective lossless compression technique used to reduce the size of data files by encoding consecutive repeated values. Here's how it works:

## Principle

- **Run-Length Encoding**: Compresses sequences of repeated data values by storing the data value and the number of times it repeats.

## Example

Given a data sequence:

```
wwwwaaadexxxxxx
```

In RLE, this sequence is encoded as:

```
w4a3d1e1x6
```

## How It Works

- **Input Sequence**: `wwwwaaadexxxxxx`
  - `w` occurs 4 times consecutively.
  - `a` occurs 3 times consecutively.
  - `d` occurs 1 time.
  - `e` occurs 1 time.
  - `x` occurs 6 times consecutively.

- **Encoded Output**: `w4a3d1e1x6`
  - Each character is followed by the count of its occurrences.

## Advantages

- **Simple**: Easy to implement and understand.
- **Effective**: Works well for data with long runs of repeated values, such as simple graphics or binary data with large homogeneous areas.

## Limitations

- **Inefficiency**: Less effective for data with few or no consecutive repeated values.
- **Overhead**: The encoding may increase the file size for data that does not have long runs of repeated values.

Run-Length Encoding is particularly useful in scenarios where data consists of long sequences of repeated values, such as in simple image formats or certain types of data logs.
