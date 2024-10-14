---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# Crypto Techniques

## Cryptography Basics

- **Cryptography**: The science of securing communication by transforming readable information into an unreadable format. It encompasses various methods and algorithms to protect sensitive data from unauthorized access and to ensure the confidentiality, integrity, and authenticity of information.
- **Plaintext**: The initial, human-readable format of data. This is the information that needs to be secured before any cryptographic operation is performed. For instance, a plaintext message could be "Meet me at the park at noon."
- **Ciphertext**: The output of the encryption process, which transforms plaintext into a format that is unreadable without the correct decryption key. For example, the plaintext "Meet me at the park at noon" might become "Ujfq dg rj wjbql gb sllq" when encrypted.
- **Key**: A critical component in cryptographic operations, keys are strings of bits used by encryption algorithms to perform encryption and decryption. The security of cryptographic systems often hinges on the secrecy and complexity of the key. For example, in a symmetric key system, both the sender and receiver must share the same secret key.

## What is Encryption?

- **Definition**: Encryption is the process of converting plaintext into ciphertext to hide the actual meaning of the information from unauthorized users. This transformation requires special knowledge (a key) to reverse the process and retrieve the original information.
- **Examples of Encryption Algorithms**:
    - **AES (Advanced Encryption Standard)**: A widely adopted symmetric encryption algorithm that offers strong security and is used globally to secure data.
    - **3DES (Triple Data Encryption Standard)**: An enhancement of DES that applies the DES algorithm three times to each data block for increased security.
    - **RC4**: A stream cipher known for its simplicity and speed but is less secure compared to AES and is now considered obsolete for many applications.
    - **ROT-13**: A simple letter substitution cipher that replaces a letter with the 13th letter after it in the alphabet, mainly used for obscuring text.

## Cryptography

Cryptography is an essential aspect of modern digital security, employing various techniques to ensure data confidentiality, integrity, and authenticity. Below are some fundamental cryptographic techniques:

- **[[Monoalphabetic Substitution-Based Ciphers]]**: This method involves replacing characters in a plaintext message with different characters based on a defined key. Each letter corresponds to a unique substitution, making it essential for the key to be kept secret for effective encryption.
    
- **[[Steganography]]**: Unlike traditional encryption, which alters the content of a message, steganography involves hiding information within seemingly ordinary messages or documents. This technique makes the presence of the secret message invisible, as it does not alert potential interceptors.
    
- **[[Enigma Technology]]**: Developed in the early 20th century, the Enigma machine utilized a complex series of rotating rotors to encrypt messages. It was famously used during World War II for secure communications and represented a significant advancement in cryptographic technology.
    
- **[[Symmetric Key Cryptography]]**: In this technique, both the sender and recipient share a single secret key used for both encryption and decryption. The security of symmetric key cryptography relies on the secrecy of the key, and any compromise can lead to unauthorized access.
    
- **[[Message Integrity Code (MIC)]]**: Also known as Message Authentication Code (MAC), this mechanism ensures the integrity of transmitted messages. It involves a key to verify that a message has not been altered during transmission, distinguishing it from standard hashing techniques.
    
- **[[Public Key Cryptography (PKC)]]**: This revolutionary technique employs a pair of keys—a public key for encryption and a private key for decryption. The beauty of PKC lies in its security; even if the public key is known, the private key remains confidential, enabling secure communications over insecure channels.
    
- **[[Web of Trust]]**: A decentralized model for establishing trust in public key cryptography, the Web of Trust allows users to vouch for one another's public keys rather than relying on a centralized Certificate Authority. This approach promotes user-driven security and flexibility.
    
- **[[Kerberos]]**: This network authentication protocol uses tickets to enable secure communication in distributed environments. It provides mutual authentication, ensuring that both clients and servers verify each other's identities, and supports single sign-on capabilities for convenient access to multiple services.