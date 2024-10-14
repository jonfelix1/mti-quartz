---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Making Connection Efficient]]"
---

# Lossy Image Compression

**Lossy Image Compression** is a technique used to reduce the file size of images by removing some of the data, which may result in a loss of quality. Here’s a detailed look at how lossy compression works, particularly focusing on JPEG:

## Basics of Image Compression

- **Image Representation**:
  - **Color Images**: Typically defined by red, green, and blue (RGB) values.
  - **Color Models**: Can also be represented using luminance and chrominance components.
  - **Bit Depth**: Each color component is usually 8 bits, resulting in a total of **24 bits** per pixel, allowing for **16,777,216 colors**.

## JPEG Compression

- **JPEG (Joint Photographic Experts Group)**: A popular format for compressing still images using lossy compression. JPEG compression involves three main phases:

### 1. Discrete Cosine Transformations (DCT)
- **Purpose**: Converts the image into numerical values by transforming spatial domain data into frequency domain data.
- **Process**: Breaks the image into blocks (e.g., 8x8 pixels) and applies the DCT to each block, representing image data as a combination of frequencies.

### 2. Quantization
- **Purpose**: Maps the continuous DCT values into discrete values.
- **Process**: Reduces the precision of the frequency data, which reduces the amount of data needed to represent the image but introduces loss. Higher frequencies (less noticeable details) are typically quantized more aggressively.

### 3. Run-Length Encoding
- **Purpose**: Compresses the quantized data by encoding sequences of repeated values.
- **Process**: Converts the quantized values into a string format that represents patterns, reducing the overall size of the data.

## Reconstructing the Image

- **Undo Run-Length Encoding**: Converts the compressed data back into its quantized form.
- **Obtain Quantized Values**: Extract the quantized values from the run-length encoded data.
- **Apply Inverse DCT**: Use the inverse of the cosine transformations to reconstruct the image from the quantized frequency data. This results in a reduced-quality image compared to the original.

## Summary

- **Lossy Compression**: Reduces file size by removing some data, which may affect quality.
- **JPEG**: Utilizes DCT, quantization, and run-length encoding to compress images.
- **Reconstruction**: Involves reversing the compression steps to obtain a reduced-quality image.

Lossy compression, such as JPEG, is widely used for images where a balance between file size and quality is needed. It achieves high compression ratios but with some loss of detail, making it suitable for applications where exact reproduction is not critical.
