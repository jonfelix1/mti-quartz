---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Making Connection Efficient]]"
---

# Lossy Compression

**Lossy Compression** is a data compression technique that reduces file size by permanently removing some data, resulting in a loss of quality. This method is often used where reduced file sizes are more critical than retaining the original quality.

## Principles

- **Data Reduction**: Compresses data by discarding less important information that is less noticeable or redundant.
- **Quality Trade-Off**: Accepts a loss of data fidelity to achieve smaller file sizes, which can affect the quality of the reconstructed data.

## Common Applications

- **Images**: Used in formats like JPEG to compress photographic images by removing less visually significant details.
- **Audio**: Applied in formats like MP3 or AAC to reduce the file size of audio by eliminating parts of the audio that are less audible.
- **Video**: Employed in codecs like H.264 or HEVC to compress video files by removing redundant information and details.

## Key Techniques

### 1. **Quantization**
- **Purpose**: Reduces the precision of the data, discarding less critical information.
- **Example**: In JPEG compression, high-frequency details (less noticeable) are quantized more aggressively than low-frequency details.

### 2. **Transform Coding**
- **Purpose**: Converts data into a different domain where redundancy can be reduced more effectively.
- **Example**: Discrete Cosine Transform (DCT) is used in JPEG compression to transform image data into frequency domain.

### 3. **Perceptual Coding**
- **Purpose**: Removes data that is less perceptible to human senses.
- **Example**: MP3 compression uses psychoacoustic models to remove sounds that are less audible to the human ear.

## Advantages

- **Significant Size Reduction**: Achieves much smaller file sizes compared to lossless compression.
- **Efficient Transmission and Storage**: Ideal for applications where bandwidth and storage are limited.

## Limitations

- **Quality Loss**: Some original data is permanently lost, which can degrade quality, especially at high compression rates.
- **Artifacts**: Can introduce visual or auditory artifacts, such as blurring in images or distortion in audio.

## Examples
- [[Lossy Audio Compression]]
- [[Lossy Video Compression]]
- [[Lossy Video Compression]]

## Summary

- **Lossy Compression**: Reduces file size by removing some of the original data, resulting in a trade-off between file size and quality.
- **Techniques**: Includes quantization, transform coding, and perceptual coding.
- **Applications**: Widely used in image, audio, and video formats where reduced file size is prioritized over perfect fidelity.

Lossy compression is essential in managing data for applications where minimizing file size is critical and some loss of quality is acceptable.
