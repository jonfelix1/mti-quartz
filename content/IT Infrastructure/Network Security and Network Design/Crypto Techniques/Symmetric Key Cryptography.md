---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# Symmetric Key Cryptography

- **Definition**: A form of encryption where the same key (known as a symmetric key) is used for both the encryption and decryption of messages. This type of cryptography requires both parties to have access to the same key to communicate securely.
- **Example**: In a monoalphabetic substitution cipher, both Bob and Alice must know the key to correctly encode and decode messages.
- **Challenge**: The main challenge of symmetric key cryptography lies in the secure exchange of keys. If a malicious actor intercepts the key during transmission, they can decrypt the messages meant for the legitimate parties.

### Data Encryption Standard (DES)

- **Introduction**: Developed in the 1970s and adopted as a federal standard in the U.S., DES encrypts data in 64-bit blocks through a series of 16 rounds, utilizing a 56-bit key.
- **Key Size**: Although a 56-bit key provides over 72 quadrillion possible combinations, advances in computing power have rendered it vulnerable to brute-force attacks.
- **Security Vulnerability**: In 1998, the Electronic Frontier Foundation cracked DES in just three days, demonstrating its susceptibility to modern attack methods.
- **Enhancements**: **3DES (Triple DES)** was introduced as a more secure alternative by applying the DES algorithm three times to each block of data, significantly increasing security but also the computational load.

### Advanced Encryption Standard (AES)

- **Selection**: In 2001, AES was selected by the National Institute of Standards and Technology (NIST) to replace DES due to its superior security features.
- **Advantages**:
    - Uses a variable key length of 128, 192, or 256 bits, providing flexibility and robust security.
    - Efficiently encrypts data using a single pass, unlike the multiple rounds in DES.
    - Suitable for a wide range of applications, from small devices to high-performance computing systems.
- **Key Space**: With a key space of 22562^{256}2256, AES provides immense security against brute-force attacks. The estimated cracking time for AES-256 is approximately 149 trillion years using current technology.
