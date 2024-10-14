---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# Wired Equivalent Privacy (WEP)

- **Definition**: WEP is a security protocol designed to provide a wireless local area network (WLAN) with a level of security and privacy comparable to what is usually expected of a wired LAN.
    
- **Key Features**:
    
    - **Encryption**: WEP uses the RC4 stream cipher for encrypting data.
    - **Static Keys**: WEP relies on a shared secret key that is typically 40 bits or 104 bits long, which is used for both encryption and decryption.
    - **Initialization Vector (IV)**: A 24-bit IV is combined with the shared secret key to produce a unique key stream for encryption.
- **Operation**:
    
    - Data is encrypted by performing an XOR operation between the plaintext data and the generated key stream from the combination of the shared secret key and the IV.
    - Each packet contains the IV, which is sent in clear text along with the encrypted data.
- **Advantages**:
    
    - Provides a basic level of security for wireless networks.
    - Relatively simple to implement and configure.
- **Drawbacks**:
    
    - **Weak Security**: The static key can be easily intercepted, and the short key length (especially the 40-bit version) makes it vulnerable to brute-force attacks.
    - **IV Reuse**: Since the IV is short (24 bits), it can be reused frequently, leading to vulnerabilities and key recovery attacks.
    - **No Mutual Authentication**: WEP does not provide a mechanism for mutual authentication between the client and the access point.
- **Legacy Status**:
    
    - Due to its numerous vulnerabilities, WEP is considered obsolete and has been largely replaced by more secure protocols like Wi-Fi Protected Access (WPA) and WPA2.
    - Modern wireless networks are advised to use WPA2 or WPA3 to ensure robust security.
- **Historical Context**:
    
    - Developed in the late 1990s as part of the IEEE 802.11 standard for wireless networks.
    - It was the first security protocol for WLANs, but its weaknesses were discovered soon after its implementation.