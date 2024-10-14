---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# Network Security

Network security encompasses a range of technologies, policies, and practices designed to protect networks from unauthorized access, misuse, or damage. Various components play a crucial role in ensuring the integrity, confidentiality, and availability of networked resources.

## Network Firewall

Firewalls are essential components of network security that filter incoming and outgoing traffic based on predetermined security rules. They can be categorized into two main types:

- **[[Router Bridge Based Firewall]]**
  - Operates on a bridge or router to protect a network or a group of devices.
  - Cisco provides firewall features integrated into their IOS operating system.

- **[[Computer-Based Firewall]]**
  - Runs on a computer, such as a PC or Unix system.
  - Free products include IPFilter, PF (from OpenBSD 3.0 and later), and IPTables (found in Linux).
  - Commercial options include Checkpoint Firewall-1, while Apple OSX includes IPFW as part of its operating system.

### Why Use a Firewall

Firewalls protect a wide range of machines from general probes and attacks, even those machines that lack inherent security measures. They serve as a barrier between trusted internal networks and untrusted external networks.

## How Does a Firewall Work?

Firewalls block packets based on several criteria:

- **Source IP Address** or range of addresses
- **Source IP Port**
- **Destination IP Address** or range of addresses
- **Destination IP Port**

Some firewalls also filter traffic at higher layers of the OSI model, allowing more advanced filtering options.

### Common Ports

- **80**: HTTP
- **443**: HTTPS
- **20 & 21**: FTP (File Transfer Protocol)
- **23**: Telnet
- **22**: SSH (Secure Shell)
- **25**: SMTP (Simple Mail Transfer Protocol)

### Sample Rules

Consider the following sample rules, where processing stops when a rule matches a packet:

1. Pass in on $external from any proto tcp to 134.71.1.25 port = 80
2. Pass in on $external from any proto tcp to 134.71.1.25 port = 53
3. Pass in on $external from any proto udp to 134.71.1.25 port = 53
4. Pass in on $external from any proto tcp to 134.71.1.25 port = 25
5. Block in log on $external from any to 134.71.1.25
6. Block in on $external from any to 134.71.1.0/24
7. Pass in on $external from any proto tcp to 134.71.1.25 port = 22
8. Pass out on $internal from 134.71.1.0/24 to any keep state

In this case, the SSH rule would never be evaluated due to the blocking rules above it.

## Transport-Layer Security (TLS)

Transport-Layer Security (TLS) is a widely deployed security protocol designed to provide secure communications over a computer network, commonly used for secure web browsing (HTTPS) on port 443. TLS ensures:

- **Confidentiality**: Achieved through symmetric encryption.
- **Integrity**: Guaranteed by cryptographic hashing.
- **Authentication**: Established via public key cryptography.

### History of TLS

- Early research and implementation began with secure network programming and secure sockets.
- The Secure Socket Layer (SSL) has been deprecated since 2015, with TLS 1.3 defined in RFC 8846 in 2018.

### What’s Needed for TLS?

- **Handshake**: Clients (Alice) and servers (Bob) use their certificates and private keys to authenticate each other and create or exchange a shared secret.
- **Key Derivation**: Shared secrets are used to derive encryption keys.
- **Data Transfer**: Data is transferred in a series of records rather than as a one-time transaction.
- **Connection Closure**: Special messages are exchanged to securely close the connection.

## Cryptographic Keys in TLS

Using different keys for various cryptographic functions is considered best practice. The following keys are derived from the key derivation function (KDF):

- **Kc**: Encryption key for data sent from client to server.
- **Mc**: MAC key for data sent from client to server.
- **Ks**: Encryption key for data sent from server to client.
- **Ms**: MAC key for data sent from server to client.

### Encrypting Data

TLS encrypts data in-stream using a series of “records,” each containing a MAC created using the corresponding MAC key. This method allows for integrity checks as data arrives, rather than waiting for the entire transmission to complete.

## IPsec

IPsec (Internet Protocol Security) provides a framework for securing communications over IP networks. It operates in two modes:

- **Transport Mode**: Only the datagram payload is encrypted and authenticated.
- **Tunnel Mode**: The entire datagram is encapsulated in a new datagram with a new IP header.

### Two IPsec Protocols

1. **Authentication Header (AH)**: Provides source authentication and data integrity but not confidentiality.
2. **Encapsulation Security Protocol (ESP)**: Offers source authentication, data integrity, and confidentiality. ESP is more widely used than AH.

### Security Associations (SAs)

Before data transmission, a security association (SA) is established, which contains state information about the encryption method, keys, and other parameters necessary for secure communication.

## Wireless Security

Securing wireless networks is vital due to their susceptibility to interception. 

- **[[Wired Equivalent Privacy (WEP)]]**: The first security protocol for wireless LANs, WEP is based on the RC4 algorithm but is now considered insecure due to its weak 40-bit keys and static keys, making it vulnerable to attacks.
  
- **[[Wi-Fi Protected Access (WPA)]]**: Replaces WEP with improved dynamic key encryption and mutual authentication mechanisms for wireless clients.
  
- **[[Wi-Fi Protected Access II (WPA2)]]**: Incorporates the Advanced Encryption Standard (AES) and supports dynamically assigned keys and encryption algorithms, ensuring a more secure wireless environment.

### Common WPA Operations

- **Pre-shared Key (PSK)**: For personal use.
- **802.1x/EAP**: For enterprise environments, involving phases such as discovery, authentication, key distribution, and management.
