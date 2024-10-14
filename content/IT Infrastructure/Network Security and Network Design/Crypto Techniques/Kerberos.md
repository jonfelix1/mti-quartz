---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# Kerberos

- **Overview**: Kerberos is a network authentication protocol designed to provide secure communication in a distributed environment. It was developed at MIT and is widely used for authenticating users and services within networks.
- **Key Components**:
    - **Key Distribution Center (KDC)**: The central component of Kerberos that issues tickets for authentication. It consists of two parts:
        - **Authentication Server (AS)**: Verifies user credentials and issues a Ticket Granting Ticket (TGT).
        - **Ticket Granting Server (TGS)**: Issues service tickets based on the TGT for accessing specific services.
    - **Tickets**: Encrypted data that allows users to prove their identity without repeatedly sending passwords over the network. Users request a TGT from the AS, which they can then use to obtain service tickets from the TGS for accessing various services.
- **Security Features**:
    - **Mutual Authentication**: Both the client and server authenticate each other, ensuring that sensitive information is only shared with legitimate parties.
    - **Single Sign-On (SSO)**: Once authenticated, users can access multiple services without needing to log in again for each one.
    - **Session Keys**: Kerberos generates temporary session keys for secure communication between clients and servers, enhancing security by limiting the exposure of long-term keys.
