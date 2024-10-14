---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Making Connection Efficient]]"
---

# Lossy Video Compression

**Video Compression** is a technique used to reduce the size of video files by removing redundant or unnecessary data, making it easier to store and transmit video content. This process involves encoding and decoding video data to achieve smaller file sizes while maintaining acceptable quality.

## Principles

- **Data Reduction**: Compresses video by eliminating redundant information within and between frames.
- **Quality vs. Size**: Balances the trade-off between video quality and file size. Higher compression typically results in more quality loss but smaller files.

## Key Techniques

### 1. **Spatial Compression**
- **Purpose**: Reduces redundancy within individual frames.
- **Method**: Applies techniques such as Discrete Cosine Transform (DCT) to convert spatial data into frequency data, which is then quantized and encoded.
- **Example**: JPEG compression for still images.

### 2. **Temporal Compression**
- **Purpose**: Reduces redundancy between consecutive frames.
- **Method**: Focuses on encoding only the differences between frames, rather than storing each frame in its entirety.
- **Example**: Differential encoding, where only changes from the previous frame are stored.

## Video Compression Standards

- **H.264 (AVC - Advanced Video Coding)**:
  - **Compression**: Uses both spatial and temporal compression techniques to achieve high compression efficiency.
  - **Features**: Widely used for streaming, Blu-ray discs, and video conferencing due to its good balance between quality and file size.

- **H.265 (HEVC - High Efficiency Video Coding)**:
  - **Compression**: Provides improved compression efficiency compared to H.264, reducing file sizes by up to 50% while maintaining similar quality.
  - **Features**: Used for 4K and high-definition video streaming and storage.

- **VP8/VP9**:
  - **Compression**: Developed by Google, VP8 is used for web video streaming, and VP9 offers improvements over VP8 with better compression efficiency.
  - **Features**: VP9 is often used in YouTube and other streaming platforms as an alternative to H.265.

- **AV1**:
  - **Compression**: A newer codec designed to provide even better compression efficiency than HEVC.
  - **Features**: Open-source and royalty-free, intended for high-definition and 4K streaming.

## Compression Process

1. **Encoding**:
   - **Transform**: Convert video data into frequency domain.
   - **Quantization**: Reduce precision of the transformed data.
   - **Encoding**: Compress data using techniques like entropy coding.

2. **Decoding**:
   - **Reverse Encoding**: Decompress encoded data.
   - **Inverse Quantization**: Restore data to its quantized form.
   - **Inverse Transform**: Convert frequency data back to spatial domain to reconstruct the video.

## Advantages

- **Efficient Storage**: Reduces the amount of data needed to store video files.
- **Faster Transmission**: Facilitates quicker streaming and downloading of video content.
- **Cost Savings**: Reduces bandwidth usage and storage costs.

## Limitations

- **Quality Loss**: Some loss of quality can occur, especially with higher compression settings.
- **Processing Requirements**: Compression and decompression require computational resources, which may impact performance.

## Summary

- **Video Compression**: Reduces video file size by removing redundancy within and between frames, using techniques like spatial and temporal compression.
- **Standards**: Common codecs include H.264, H.265, VP8/VP9, and AV1, each with varying levels of efficiency and quality.
- **Applications**: Used in streaming, storage, and broadcasting to optimize video delivery and management.

Video compression is essential for managing large video files, optimizing streaming performance, and reducing storage and bandwidth costs while striving to maintain acceptable video quality.
