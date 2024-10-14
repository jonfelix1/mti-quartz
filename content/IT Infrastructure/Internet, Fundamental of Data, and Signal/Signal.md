---
tags:
  - note
  - inti
Class: "[[IT Infrastructure Class (INTI)]]"
---

# Signals

Signals are essential in telecommunications and data transmission, characterized by three primary components: **Amplitude**, **Frequency**, and **Phase**.

## Amplitude
- **Amplitude** refers to the height of the wave above or below a reference point.
- It is typically measured in **volts**.

## Frequency
- **Frequency** indicates how many times a signal completes a cycle in a specific time frame, measured in **Hertz (Hz)**, or cycles per second.
  - **Period** is calculated as \( \text{Period} = \frac{1}{\text{Frequency}} \).
- The **spectrum** represents the range of frequencies a signal spans, from its minimum to maximum values.
- **Bandwidth** is defined as the absolute difference between the lowest and highest frequencies of a signal.

### Example: Average Voice
- The average voice operates within a frequency range of approximately **300 Hz to 3100 Hz**.
  - The spectrum would be **300 – 3100 Hz**.
  - The bandwidth would be **2800 Hz**.

## Phase
- **Phase** describes the position of a waveform concerning a specific moment in time or relative to time zero.
- Phase can change by any angle between **0 and 360 degrees**, with common phase angles being 45, 90, 135, etc.
  
### Phase and Signal Transmission
- If a signal can demonstrate two different phase angles, **1 bit** can be transmitted with each signal change (or baud).
- If it can exhibit four different phase angles, then **2 bits** can be transmitted with each change.
- The relationship can be expressed mathematically as:
  $$
  \text{Number of bits transmitted} = \log_2(\text{Number of different phase angles})
  $$
- This principle also applies to **amplitude levels** or **frequency levels**.

## Decibels (dB)
- The **decibel (dB)** is a logarithmic unit used to express the ratio of two values, commonly in power.
- The formula for calculating decibels is:
  $$
  \text{dB} = 10 \times \log_{10} \left(\frac{P_2}{P_1}\right)
  $$
  where $P_1$ is the initial power level, and $P_2$ is the final power level.

### Loss of Signal Strength (in dB)
- To determine the impact of a signal loss:
  - If a signal loses **3 dB**, how significant is that?
  - For a signal starting at **100 watts** and ending at **50 watts**, the dB loss can be calculated as follows:
  $$
  \text{dB} = 10 \times \log_{10} \left(\frac{50}{100}\right) = 10 \times \log_{10}(0.5) \approx 10 \times -0.3 = -3.0
  $$
- Therefore, a **3 dB loss** indicates that the signal has lost half of its power.

Understanding these fundamentals of signals is crucial for effective communication and data transmission in various technological applications.


