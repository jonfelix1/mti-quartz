---
tags:
  - inti
  - note
  - topic
Class: "[[IT Infrastructure Class (INTI)]]"
---

# Noise and Error Sources in [[Communication Media]]

Noise and errors are critical factors that can affect the reliability and quality of data transmission in communication networks. Below are important concepts related to noise and error management:

## Types of Noise

- **[[White Noise]]**: A type of noise that contains a wide range of frequencies, typically affecting all channels equally, leading to random interference in the communication signal.
    
- **[[Impulse Noise]]**: Short-duration, high-amplitude noise spikes that can cause significant disruptions in signal integrity, often resulting from electrical disturbances or switching actions.
    
- **[[Crosstalk]]**: Unwanted transfer of signals between communication channels, which can lead to interference and degradation of data transmission quality.
    
- **[[Echo]]**: A reflection of transmitted signals that returns to the sender, causing confusion and errors in data interpretation, particularly in voice communications.
    
- **[[Attenuation]]**: The reduction in signal strength as it travels through a medium, leading to potential data loss or degradation if the signal becomes too weak.
    
- **[[Delay Distortion]]**: Variations in the time taken for different frequency components of a signal to travel through a medium, which can lead to signal distortion and errors.
    

## Error Detection and Correction

- **[[Error Detection]]**: Techniques used to identify errors in transmitted data, ensuring that data integrity is maintained during communication.
    
- **[[Error Control]]**: A broad set of techniques used to manage errors in data transmission, encompassing both detection and correction methods.
    
- **[[Error Correction]]:** Methods that not only detect errors but also correct them, allowing for reliable data transmission without requiring retransmission.
    
- **[[Hamming Code]]**: A specific error-correcting code that can detect and correct single-bit errors in data transmissions, enhancing reliability in communication.
    
- **[[Cyclic Redundancy Checksum (CRC)]]**: A widely used error-detecting code that generates a fixed-size checksum based on the data being transmitted, helping to identify errors in data integrity.
    
- **[[Longitudinal Parity Check]]**: A method that adds parity bits to data blocks to detect errors, allowing for simple error detection based on the parity of the transmitted data.
    
- **[[Parity Check]]**: A basic error detection technique that uses a single parity bit to indicate whether the number of set bits in a binary sequence is even or odd.
    

## Error Management Techniques

- **[[Do Nothing - Toss the Frame or Packet]]**: A strategy where corrupted frames or packets are discarded without attempting recovery, relying on higher-layer protocols to manage retransmission.
    
- **[[Return A Message]]**: A technique where the receiving end sends a message back to the sender to indicate receipt of data or to report errors.
    
- **[[Sliding Window Error Control]]**: A flow control method that allows multiple frames to be in transit before needing an acknowledgment, improving efficiency while managing errors.
    
- **[[Stop-and-Wait Error Control]]**: A simpler error control method where the sender transmits one frame and waits for acknowledgment before sending the next, ensuring data integrity but reducing throughput.
    
- **[[Jitter]]**: The variation in packet arrival times, which can cause issues in time-sensitive applications like streaming or VoIP, impacting overall data transmission quality.