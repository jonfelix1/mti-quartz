---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# Monoalphabetic Substitution-Based Ciphers

- **Overview**: Monoalphabetic substitution ciphers replace each letter in the plaintext with a corresponding letter from a different alphabet (the key). This simple substitution can be effective, but its security is limited due to the predictable nature of the replacement.
- **Example**:
    - **Replacement Alphabet**:
        - Original: `abcdefghijklmnopqrstuvwxyz`
        - Key: `POIUYTREWQLKJHGFDSAMNBVCX`
    - **Encoding**: The plaintext "how about lunch at noon" encodes to "EGVPO GNMKN HIEPM HGGH" using the substitution.
- **Strength**: The key space for a monoalphabetic cipher is relatively small (limited to the number of letters in the alphabet), making it susceptible to frequency analysis attacks. For example, the letter "e" is the most common letter in English and can be easily identified in ciphertext.
- **Historical Example**: The **Caesar Cipher**, attributed to Julius Caesar, is a specific type of monoalphabetic substitution cipher where each letter is shifted a fixed number of places down the alphabet (e.g., a shift of 3 transforms "A" to "D").
