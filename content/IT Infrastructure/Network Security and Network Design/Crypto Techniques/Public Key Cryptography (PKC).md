---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# Public Key Cryptography (PKC)

- **Overview**: Public key cryptography revolutionized secure communication by introducing two distinct keys: a public key for encryption and a private key for decryption. This method eliminates the need for both parties to share a secret key, making secure communication more feasible.
- **Security Properties**:
    - The public key can be shared openly without compromising security, as the corresponding private key is never shared.
    - It is computationally infeasible to derive the private key from the public key, ensuring the security of the encryption process.

### Public Key Infrastructure (PKI)

- **Definition**: A comprehensive framework that encompasses the technologies, policies, and procedures required to manage digital certificates and public key encryption. PKI enables secure communication over networks.
- **Digital Certificates**: Electronic documents that bind a public key to an entity's identity, providing assurance of the key owner's legitimacy. Digital certificates include:
    - The subject's name, a unique serial number, validity dates, the public key, and the digital signature of the issuing Certificate Authority (CA).
- **Certificate Authorities (CAs)**: Trusted entities responsible for issuing and managing digital certificates. They validate the identity of certificate applicants and provide assurance that public keys belong to the specified entities.