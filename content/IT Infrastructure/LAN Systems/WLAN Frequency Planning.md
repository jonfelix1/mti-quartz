---
tags:
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Local Area Network (LAN)]]"
---

# WLAN Frequency Planning

## Overview

- **WLAN Frequency Planning** involves the strategic allocation and management of radio frequencies to ensure optimal performance and minimize interference in wireless local area networks (WLANs).
- Effective frequency planning is crucial for maintaining high network performance, reliability, and coverage.

## Key Considerations

### Frequency Bands

- **2.4 GHz Band**:
  - **Channels**: 11-14 channels (depending on the region).
  - **Bandwidth**: Each channel has a bandwidth of 20 MHz.
  - **Channel Overlap**: Channels overlap significantly, leading to potential interference. Non-overlapping channels typically used are 1, 6, and 11.

- **5 GHz Band**:
  - **Channels**: More channels available compared to 2.4 GHz, with less overlap.
  - **Bandwidth**: Channels can be 20 MHz, 40 MHz, 80 MHz, or 160 MHz wide.
  - **Regulations**: Varies by region; includes additional channels for higher speeds and less interference.

### Channel Allocation

- **Non-Overlapping Channels**:
  - For the 2.4 GHz band, use channels 1, 6, and 11 to avoid overlap and interference.

- **Channel Width**:
  - Wider channels (e.g., 40 MHz, 80 MHz) offer higher data rates but are more prone to interference. Balance between data rate and interference is necessary.

### Interference Management

- **Adjacent-Channel Interference**:
  - Use non-overlapping channels to minimize interference from adjacent channels.

- **Co-Channel Interference**:
  - Ensure adequate distance between access points using the same channel to reduce co-channel interference.

- **External Interference**:
  - Identify and mitigate interference from non-WLAN sources (e.g., microwave ovens, cordless phones).

### Access Point Placement

- **Density**:
  - Proper placement of access points (APs) to ensure sufficient coverage without excessive overlap.
  - Avoid placing APs too close to each other to minimize interference.

- **Coverage**:
  - Ensure uniform coverage by considering the physical layout and potential obstacles (walls, furniture) that can affect signal propagation.

## Tools and Techniques

### Site Surveys

- **Site Survey**:
  - Conduct surveys to assess the physical environment, identify sources of interference, and determine optimal AP placement.

- **Tools**:
  - Use spectrum analyzers and WLAN planning software to analyze frequency usage and plan channel allocations.

### Dynamic Frequency Selection (DFS)

- **DFS**:
  - Automatically selects channels to avoid interference with radar systems and other priority users.

### Channel Bonding

- **Channel Bonding**:
  - Combine multiple channels to increase bandwidth (e.g., 40 MHz, 80 MHz, 160 MHz) while managing potential interference.

## Summary

- **WLAN Frequency Planning** is essential for optimizing network performance and reducing interference.
- Key aspects include selecting appropriate frequency bands, channel allocation, interference management, and proper AP placement.
- Utilize tools like site surveys and spectrum analyzers to ensure effective planning and deployment.


