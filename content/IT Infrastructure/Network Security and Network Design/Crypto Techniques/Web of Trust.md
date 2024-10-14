---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# Web of Trust

- **Concept**: The Web of Trust is a decentralized model for establishing a network of trust among users in public key cryptography. Unlike traditional public key infrastructures (PKI) that rely on a centralized Certificate Authority (CA), the Web of Trust allows users to vouch for one another's public keys.
- **Mechanism**:
    - Users can create digital signatures for others' public keys, establishing a chain of trust based on personal relationships and endorsements. If Alice trusts Bob's key and signs it, others who trust Alice can also trust Bob's key.
    - The degree of trust is subjective; users can assign varying levels of trust to different keys based on their knowledge and interactions with those users.
- **Applications**: The Web of Trust is commonly used in PGP (Pretty Good Privacy) for email encryption, allowing individuals to manage their own keys without relying on a central authority. This model can foster more flexible and user-driven security practices.