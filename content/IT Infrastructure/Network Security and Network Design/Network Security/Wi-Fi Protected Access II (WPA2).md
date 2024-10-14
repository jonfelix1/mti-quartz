---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# Wi-Fi Protected Access II (WPA2)

- **Definition**: WPA2 is an enhanced version of Wi-Fi Protected Access (WPA) designed to provide stronger security for wireless networks, utilizing the Advanced Encryption Standard (AES) for encryption.

- **Key Features**:
  - **Advanced Encryption Standard (AES)**: WPA2 employs AES, a symmetric key encryption algorithm that is considered more secure than the Temporal Key Integrity Protocol (TKIP) used in WPA.
  - **Mandatory Support for AES**: Unlike WPA, which could use TKIP, WPA2 mandates the use of AES for encryption, ensuring a higher level of data protection.
  - **Two Modes of Operation**:
    - **Personal Mode (PSK)**: Utilizes a pre-shared key for authentication, making it suitable for home networks and small businesses.
    - **Enterprise Mode (802.1X)**: Employs a RADIUS server for authentication, allowing for more complex security measures suitable for larger organizations.

- **Operation**:
  - **Encryption**: Data is encrypted using AES in Counter Mode with Cipher Block Chaining Message Authentication Code (CCMP), ensuring data confidentiality and integrity.
  - **Authentication**: The authentication process can be performed using either a simple password (in Personal mode) or more sophisticated methods through an authentication server (in Enterprise mode).

- **Advantages**:
  - **Robust Security**: Offers significant improvements in security compared to both WEP and WPA, making it resistant to various attack methods.
  - **Support for Multiple Users**: The Enterprise mode allows for individual user credentials, enhancing security by limiting access based on user identity.
  - **Data Integrity**: CCMP ensures data integrity and authenticity, protecting against tampering and forgery.

- **Drawbacks**:
  - **Complexity**: The setup for WPA2 Enterprise can be complex, requiring additional infrastructure such as RADIUS servers.
  - **Performance**: While generally efficient, the use of AES may introduce some performance overhead, particularly on older hardware.

- **Legacy Status**:
  - WPA2 has been the standard for wireless security since its introduction in 2004 and is widely supported by all modern Wi-Fi devices.
  - Although WPA3 has been introduced as the successor to WPA2, many networks continue to use WPA2 due to its proven security features.

- **Historical Context**:
  - Developed by the Wi-Fi Alliance to address vulnerabilities in earlier wireless security protocols and establish a more secure standard for wireless networking.
  - WPA2 became the mandatory security standard for Wi-Fi networks, significantly improving the overall security of wireless communications.