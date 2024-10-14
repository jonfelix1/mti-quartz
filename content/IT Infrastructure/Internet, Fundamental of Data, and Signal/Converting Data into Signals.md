---
tags:
  - note
  - inti
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Internet, Fundamental of Data, and Signal]]"
---

# Converting Data into Signals

Data conversion into signals is essential for effective communication in digital and analog systems. This process can occur through various combinations, which primarily include the following:

- **Analog data transmitted using analog signals.**
- **Digital data transmitted using digital signals.**
- **Digital data transmitted using discrete analog signals.**
- **Analog data transmitted using digital signals.**

Each method has specific applications, advantages, and technologies associated with it. Below is an in-depth exploration of these combinations.

## 1. Transmitting Analog Data with Analog Signals

### Modulation Techniques
To transmit analog data effectively, it is often necessary to **modulate** this data onto a set of analog signals. This process enables efficient transmission over various media, allowing for the coexistence of multiple channels. Here are common applications:

- **Broadcast Radio**: Uses amplitude modulation (AM) or frequency modulation (FM) to transmit audio signals over the airwaves. Different radio stations operate on different frequencies, allowing listeners to tune into their desired channels without interference.

- **Television**: Similar to radio, older television broadcasts utilize analog signals modulated onto different frequencies to transmit video and audio content. This modulation allows viewers to access a variety of channels.

### Advantages of Analog Transmission
- **Simplicity**: Analog systems are often simpler and cheaper to implement for certain applications, particularly in traditional broadcasting.
- **Continuous Signals**: Analog signals represent data continuously, which can be beneficial for specific types of information, such as audio and video, which are naturally analog in nature.

## 2. Transmitting Digital Data with Digital Signals: Digital Encoding Schemes

When transmitting digital data, several techniques can convert this data into digital signals, making them suitable for network transmission. Common digital encoding schemes include:

### Digital Encoding Techniques
1. **NRZ-L (Non-Return to Zero-Level)**: Represents data as high or low voltage levels without returning to zero between bits. This method is simple but can face synchronization issues.

2. **NRZI (Non-Return to Zero Inverted)**: Similar to NRZ-L but changes the signal level at the beginning of each bit interval based on whether the bit is a 1 or a 0. This helps with synchronization.

3. **Manchester Encoding**: Combines clock and data signals by representing each bit with a transition; a transition in the middle of the bit period indicates a 1, while the absence of a transition indicates a 0. This encoding helps maintain synchronization.

4. **Differential Manchester Encoding**: Similar to Manchester encoding but uses transitions at the beginning of the bit period to indicate a 0 or 1, providing a way to maintain synchronization with fewer transitions.

5. **Bipolar AMI (Alternate Mark Inversion)**: Uses three voltage levels: positive, negative, and zero. A '1' is represented by alternating positive and negative voltages, while a '0' is represented by zero voltage. This encoding helps reduce the DC component of the signal.

### Applications of Digital Encoding
- **Local Area Networks (LANs)**: Digital encoding schemes are widely used in LAN technologies like Ethernet, which rely on efficient data transfer between devices.
- **Telecommunication Systems**: Digital encoding is fundamental in modern telecommunication systems, enabling reliable data transmission over various media.

## 3. Transmitting Digital Data with Discrete Analog Signals

Discrete analog signals can also carry digital data using several modulation techniques. The three primary methods include:

### Modulation Techniques
1. **Amplitude Shift Keying (ASK)**: A method where two different amplitudes represent binary digits. For example, a higher amplitude might represent a '1,' while a lower amplitude represents a '0.' ASK is simple but can be susceptible to noise.

2. **Frequency Shift Keying (FSK)**: Utilizes two different frequencies to represent binary values. One frequency denotes a '1,' while another denotes a '0.' FSK is more robust against noise than ASK and is often used in modems.

3. **Phase Shift Keying (PSK)**: Involves changing the phase of the signal to represent data. For instance, one phase shift represents a '0,' while another shift represents a '1.' 
   - **Quadrature Phase Shift Keying (QPSK)**: An advanced form of PSK that utilizes four different phase shifts (45, 135, 225, and 315 degrees), allowing it to transmit two bits per symbol, thereby increasing data rates.

### Advantages of Discrete Analog Signals
- **Resilience to Noise**: These modulation techniques are generally more resistant to noise compared to simple analog transmission methods.
- **Higher Data Rates**: Techniques like PSK and QPSK allow for higher data rates, making them suitable for modern communication systems.

## 4. Transmitting Analog Data with Digital Signals

To convert analog data into digital signals, two prominent techniques are employed: **Pulse Code Modulation (PCM)** and **Delta Modulation**. 

### Pulse Code Modulation (PCM)
PCM is a widely used method for digitizing analog signals, particularly in telecommunications.

- **Sampling**: Analog signals are sampled at regular intervals. The frequency of these samples must meet the Nyquist criterion, which states that the sampling rate should be at least twice the highest frequency present in the signal. For example, to digitize voice, typically sampled at **4000 Hz**, the required sampling rate would be **8000 samples per second**.

- **Quantization Levels**: Each sample is assigned a discrete value based on quantization levels:
  - **128 Levels**: Requires 7 bits per sample (since $2^7 = 128$).
  - **256 Levels**: Requires 8 bits per sample (since $2^8 = 256$).

- **Bit Rate Calculation**: According to the Nyquist bit rate formula:
  $$
  C = 2B \log_2 N
  $$
  where $C$ is the bit rate in bps, $B$ is the bandwidth in Hz, and $N$ is the number of levels.

### Delta Modulation
Delta modulation tracks the changes in the analog signal over time.

- **Binary Representation**: A binary '1' indicates a rise in the signal, while a '0' indicates a drop. This method is simpler than PCM but can suffer from quantization errors if the signal changes rapidly.

### Advantages of Digital Signal Transmission
- **Reduced Noise and Interference**: Digital signals are less susceptible to noise and interference, making them more reliable than analog signals.
- **Easier to Process**: Digital signals can be easily processed, manipulated, and stored using digital systems.

Understanding these methods of converting data into signals is fundamental for designing effective communication systems, whether for broadcasting, telecommunication, or data transmission across networks. These techniques enable the transfer of information in a variety of formats, allowing for efficient communication in today's digital world.