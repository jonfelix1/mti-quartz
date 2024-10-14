---
tags:
  - note
  - inti
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Internet, Fundamental of Data, and Signal]]"
---

# Data Transmission Techniques

Data transmission techniques are methods used to convey information from one location to another. These techniques can be categorized based on the nature of the data being transmitted and the type of signals used. Below is an elaboration on the four primary categories of data transmission techniques:

---

## Analog Data with Analog Signals
This technique involves modulating analog data into analog signals for transmission. It is commonly used in traditional broadcasting and communication systems.

### Modulation Techniques
- **Amplitude Modulation (AM):** The amplitude of the carrier wave is varied in accordance with the data signal. This method is widely used in AM radio broadcasting.
- **Frequency Modulation (FM):** The frequency of the carrier wave is varied according to the amplitude of the input signal. FM is commonly used for FM radio and television broadcasting due to its resistance to noise.
- **Phase Modulation (PM):** The phase of the carrier signal is varied based on the data signal. PM is often used in digital signal processing and telecommunications.

### Applications
Radio broadcasting, television signals, and other forms of analog communication rely heavily on these modulation techniques.

---

## Digital Data with Digital Signals
This technique involves encoding digital data into digital signals for transmission over a network.

### Encoding Schemes
- **Non-Return-to-Zero Level (NRZ-L):** Represents binary 1 with a high voltage level and binary 0 with a low voltage level, maintaining that level throughout the bit interval.
- **Manchester Encoding:** Combines clocking and data information; a transition occurs in the middle of each bit period where a low-to-high transition represents a binary 1, and a high-to-low transition represents a binary 0.
- **Differential Manchester Encoding:** Similar to Manchester encoding, but the presence of a transition at the beginning of the bit interval indicates a binary 0, while no transition indicates a binary 1.

### Applications
Digital signals are less susceptible to noise, making them more reliable for data transmission over long distances compared to analog signals.

---

## Digital Data with Discrete Analog Signals
In this technique, digital data is transmitted using discrete levels of an analog signal. This method is often referred to as modulation.

### Techniques
- **Amplitude Shift Keying (ASK):** Represents binary 1 by sending a higher amplitude signal and binary 0 by sending no signal or a lower amplitude signal.
- **Frequency Shift Keying (FSK):** Uses different frequencies to represent different bits; for example, one frequency for binary 1 and another for binary 0.
- **Phase Shift Keying (PSK):** Uses phase changes in a carrier wave to represent data; for instance, a phase shift could indicate a binary 1 while no shift indicates a binary 0.

### Applications
Commonly used in modems, radio communications, and wireless transmissions where digital information needs to be conveyed over an analog medium.

---

## Analog Data with Digital Signals
This technique converts analog data into digital signals for transmission. It involves sampling and quantization processes.

### Techniques
- **Pulse Code Modulation (PCM):** Involves sampling an analog signal at regular intervals and converting these samples into digital values. Each sample is quantized into discrete levels, which are then encoded into binary format for transmission.
  - *Sampling:* According to Nyquist's theorem, sampling must occur at least twice the highest frequency present in the analog signal to accurately reconstruct it.
  - *Quantization:* The process of mapping sampled values to discrete levels introduces quantization noise, which can affect signal quality.
- **Delta Modulation (DM):** A simpler form of PCM that encodes only the difference between successive samples rather than their absolute values. This technique can be more efficient but may introduce more distortion if not properly managed.

### Applications
PCM is widely used in digital telephony, audio CDs, and video compression formats.
