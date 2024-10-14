---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# Message Integrity Code (MIC)

- **Definition**: A Message Integrity Code (MIC), also known as a Message Authentication Code (MAC), is used to ensure the integrity and authenticity of transmitted messages. It verifies that a message has not been altered in transit.
- **Comparison with Hash**: While both MICs and hash functions aim to verify data integrity, MICs incorporate a secret key in their computation, ensuring that only authorized users can generate or validate the code.

### Types of Message Integrity Codes

- **HMAC (Keyed-Hash Message Authentication Code)**:
    - Utilizes a cryptographic hash function along with a secret key, providing both data integrity and authenticity.
    - Common hash functions used in HMAC include SHA-1, SHA-256, and SHA-3.
- **KMAC (KECCAK Message Authentication Code)**:
    - Based on the SHA-3 hash standard, KMAC provides keyed message authentication with additional parameters for flexibility.
    - Variants include KMAC256 and KMAC128, which differ in the output length of the message authentication code.
- **CMAC (Cipher-based Message Authentication Code)**:
    - Utilizes a symmetric block cipher, such as AES, to generate a message authentication code, ensuring both the integrity and authenticity of the message.