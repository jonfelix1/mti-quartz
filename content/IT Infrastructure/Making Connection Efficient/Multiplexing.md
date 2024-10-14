---
tags:
  - inti
  - note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Making Connection Efficient]]"
---

# Multiplexing
- **Multiplexing** allows multiple **signals** or streams of data to share the same **communication channel** simultaneously.
- This is achieved by combining signals into one **complex signal** and recovering them at the **receiving end**.
- It helps optimize the use of **communication resources**.
- Common types include:
    - [[Frequency Division Multiplexing]]: Divides the medium into distinct **frequency ranges**.
    - [[Time Division Multiplexing]]: Allocates different **time slots** for each signal.
    - [[Code Division Multiplexing]]: Each signal is assigned a unique **code** for simultaneous transmission.

## Comparison of Multiplexing Techniques

Here's a comparison of **Frequency Division Multiplexing (FDM)**, **Synchronous Time Division Multiplexing (TDM)**, **Statistical Time Division Multiplexing (STDM)**, **Wavelength Division Multiplexing (WDM)**, and **Code Division Multiplexing (CDM)**:

### [[Frequency Division Multiplexing]]

- **Principle**: Divides the frequency spectrum into non-overlapping bands, each used by a different signal.
- **Advantages**:
  - **Simple Implementation**: Each channel uses a distinct frequency band.
  - **Continuous Transmission**: Channels can transmit data continuously.
- **Disadvantages**:
  - **Interference**: Adjacent channels can interfere with each other if not properly isolated.
  - **Bandwidth Limitation**: Limited by the available frequency spectrum.

### [[Synchronous Time Division Multiplexing]]

- **Principle**: Divides time into fixed slots, assigning each slot to a different signal.
- **Advantages**:
  - **Predictable Performance**: Fixed time slots ensure that each channel gets an equal share of the bandwidth.
  - **No Interference**: Channels are separated by time, so there is no interference.
- **Disadvantages**:
  - **Inefficient**: Fixed slots may lead to wasted bandwidth if not all channels have data to send.
  - **Synchronization**: Requires precise synchronization between the sender and receiver.

### [[Statistical Time Division Multiplexing]]

- **Principle**: Similar to TDM but allocates time slots based on demand, rather than fixed slots.
- **Advantages**:
  - **Efficient Bandwidth Usage**: Allocates time slots dynamically, reducing wastage.
  - **Adaptable**: Can handle varying data rates and usage patterns.
- **Disadvantages**:
  - **Complex Implementation**: Requires algorithms to dynamically allocate slots.
  - **Variable Delay**: Data transmission delay can vary based on demand and traffic.

### [[Wavelength Division Multiplexing]]

- **Principle**: Uses different wavelengths (colors) of light to transmit multiple signals simultaneously over a single optical fiber.
- **Advantages**:
  - **High Capacity**: Can significantly increase the capacity of optical fiber systems.
  - **Low Interference**: Different wavelengths do not interfere with each other.
- **Disadvantages**:
  - **Complex Equipment**: Requires specialized optical equipment for multiplexing and demultiplexing.
  - **Cost**: Can be more expensive due to the need for advanced optical components.

### [[Code Division Multiplexing]]

- **Principle**: Assigns a unique code to each signal, allowing multiple signals to occupy the same frequency band simultaneously.
- **Advantages**:
  - **High Capacity**: Can support a large number of users in the same frequency band.
  - **Robustness**: Better resistance to interference and noise.
- **Disadvantages**:
  - **Power Control**: Requires careful power management to avoid interference between signals.
  - **Complexity**: Decoding and encoding can be complex due to the use of codes.

### Summary of Comparison

- **FDM**: Divides spectrum into frequency bands; simple but limited by spectrum and prone to interference.
- **Synchronous TDM**: Fixed time slots; predictable but potentially inefficient with idle slots.
- **Statistical TDM**: Dynamic time slot allocation; efficient but complex and variable delay.
- **WDM**: Multiple wavelengths in optical fiber; high capacity but costly and complex.
- **CDM**: Unique codes for simultaneous transmission; high capacity and robustness but complex and requires power control.

Each technique has its own strengths and is suited to different types of communication systems based on factors such as bandwidth requirements, complexity, and cost.