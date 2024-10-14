---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# Wi-Fi Protected Access (WPA)

- **Definition**: WPA is a security protocol designed to provide stronger data protection and network access control for wireless networks compared to its predecessor, Wired Equivalent Privacy (WEP).

- **Key Features**:
  - **Dynamic Key Management**: WPA uses a dynamic key management system, which means encryption keys are generated and changed automatically, reducing the risk of key compromise.
  - **Temporal Key Integrity Protocol (TKIP)**: WPA employs TKIP to enhance security by adding a per-packet key mixing function and a message integrity check (MIC) to prevent unauthorized data access and tampering.
  - **Authentication**: WPA supports both Pre-Shared Key (PSK) and IEEE 802.1X for authentication, allowing for different configurations based on network needs.

- **Operation**:
  - **Encryption**: WPA encrypts data using TKIP, which improves upon WEP's static key system by using unique keys for each data packet.
  - **Authentication**: The authentication process can be achieved through a simple password (PSK) or via a more complex setup using an authentication server with 802.1X.
  
- **Advantages**:
  - **Enhanced Security**: Provides a significant improvement over WEP in terms of encryption strength and security features.
  - **Mitigates Known Attacks**: WPA addresses many vulnerabilities identified in WEP, such as IV reuse and static key management.
  - **Backward Compatibility**: WPA was designed to be backward compatible with existing hardware that supported WEP, allowing for easier transitions to stronger security protocols.

- **Drawbacks**:
  - **Performance Overhead**: The encryption and decryption processes may introduce some performance overhead on older hardware.
  - **Still Vulnerable**: While more secure than WEP, WPA can still be susceptible to certain types of attacks (e.g., dictionary attacks on PSK).

- **Legacy Status**:
  - WPA was introduced in 2003 and has since been largely replaced by WPA2, which uses the Advanced Encryption Standard (AES) for encryption, providing even greater security.
  - WPA is considered less secure than WPA2 and is generally not recommended for new installations.

- **Historical Context**:
  - Developed by the Wi-Fi Alliance to address the vulnerabilities found in WEP and provide a more secure wireless networking standard.
  - It was a key step towards achieving stronger wireless security in consumer and enterprise environments.