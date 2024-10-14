---
tags:
- inti
- note
- topic
Class: "[[IT Infrastructure Class (INTI)]]"
---

# Routing, Internet Protocol and Services

## Overview of Networking Concepts


- **[[Types of Network Structures]]**: This provides a foundation for understanding how data is transmitted across different network architectures, such as circuit-switched and packet-switched networks.
    
- **[[Connection-Oriented vs. Connectionless Applications]]**: These applications utilize different network structures to transfer data. Connection-oriented applications, which require a dedicated connection, often operate over more reliable structures, while connectionless applications can leverage packet-switched networks for efficiency.
    
- **[[Forwarding Table]]**: A crucial component for routers and switches, the forwarding table directs packets based on the destination address. This table is built from the routing information obtained from various algorithms.
    
- **[[Forwarding Table Layer]]**: This layer operates with the forwarding table to determine how packets are directed within a network, emphasizing the relationship between routing decisions and data forwarding.
    
- **[[Hub vs Switch vs Router]]**: Understanding the differences between these devices is essential for grasping how data packets are handled in a network. Hubs broadcast signals, switches use forwarding tables to direct packets intelligently, and routers rely on routing protocols to forward data between different networks.
    
- **[[Routing vs Forwarding]]**: This concept differentiates the two fundamental operations in networking. Routing involves determining the best path for data packets, while forwarding involves moving those packets based on the predetermined routes.
    
- **[[Routing Classification]]**: Routing protocols can be classified into intradomain and interdomain categories. This classification affects how routing decisions are made and the scalability of routing protocols within different network structures.
    
- **[[Link-State Algorithm (SPF)]]**: As a dynamic routing method, the link-state algorithm computes the shortest paths in a network by using a complete view of the topology. This algorithm influences how forwarding tables are populated.
    
- **[[Static vs Dynamic Routing]]**: Static routing relies on manually configured routes, which may not adapt well to network changes, whereas dynamic routing uses algorithms like SPF to adjust to changing network conditions, leading to more efficient forwarding.
    
- **[[Telephony Routing vs Internet Routing]]**: The distinction between these two routing approaches highlights the differences in resource allocation and network stability. Telephony routing often employs static methods with resource reservations, while Internet routing utilizes dynamic protocols to adapt to varying traffic loads.
    
- **[[Basic Dynamic Routing Methods]]**: This concept covers the techniques used to exchange routing information among routers, including link-state and distance vector approaches. These methods determine how routers communicate and update their forwarding tables.
    
- **[[Routing Example]]**: Concrete examples of how routing protocols and algorithms operate help illustrate the concepts discussed in previous notes, providing practical insights into network behavior.
## Internet Protocols

### Core Protocols

> TCP vs UDP
> ![[Pasted image 20241013000520.png]]

- **[[Transmission Control Protocol (TCP)]]**: A fundamental communication protocol that ensures reliable, ordered, and error-checked delivery of data between applications running on devices in a network. It establishes a connection before data transfer and manages data segmentation and reassembly.
    
- **[[User Datagram Protocol (UDP)]]**: A simpler communication protocol that enables fast, connectionless data transfer without the reliability features of TCP. It's often used for real-time applications where speed is crucial, such as streaming and gaming.
    

### Addressing and Resolution

- **[[Address Resolution Protocol (ARP)]]**: A protocol used to map IP addresses to physical MAC addresses in a local network, allowing devices to discover the hardware address of a device given its IP address.
    
- **[[Dynamic Host Configuration Protocol (DHCP)]]**: A network management protocol that automatically assigns IP addresses and other network configuration settings to devices on a network, simplifying the management of IP address allocation.
    
- **[[Network Address Translation (NAT)]]**: A method used to translate private IP addresses within a local network to a public IP address for internet access, enhancing security and allowing multiple devices to share a single public IP address.
    

### Naming and Routing

- **[[Domain Name System (DNS)]]**: A hierarchical naming system that translates human-readable domain names (like [www.example.com](http://www.example.com)) into IP addresses, enabling browsers to load internet resources.
    
- **[[Multiprotocol Label Switching (MPLS)]]**: A high-performance routing technique that directs data from one node to another based on short path labels rather than long network addresses, improving the speed and efficiency of data flows.
    

### Web and Hosting

- **[[The World Wide Web (WWW)]]**: An information system that allows documents and resources to be accessed over the internet through hyperlinks and web browsers, using protocols like HTTP and HTTPS.
    
- **[[Web Server Basics]]**: Fundamental components of web hosting, which include a public IP address, a registered domain name, and software that serves web page files to users.
    
- **[[Web Hosting]]**: The service that allows individuals and organizations to post a website or web application onto the internet. It includes storage space on a server and services for serving web content.
    

### Advanced Networking

- **[[Tunneling Protocols and Virtual Private Networks (VPNs)]]**: Protocols that enable secure connections over the internet by encapsulating data packets within a secure tunnel, ensuring privacy and security for remote access and data transmission.

## Internet Services

The Internet offers a wide array of services that have transformed how individuals and businesses interact. Among these services, [[Internet Services]] such as electronic mail, file transfer protocols, and instant messaging facilitate seamless communication and data sharing.

A key aspect of the user experience on the Internet is [[Cookies and State Information]], which are small pieces of data created by web servers and stored on a user’s device. These cookies help track user activity and preferences, enhancing convenience in online transactions while also raising privacy concerns.

As the Internet has evolved, so has the need for effective [[Internet Governance]]. This involves the development of shared principles and norms that guide how the Internet is used and regulated by governments, private sectors, and civil society. The growth of e-commerce has made governance even more crucial, as businesses navigate the complexities of online transactions.

In addition to public access, many organizations utilize private networks known as [[Intranets and Extranets]]. An intranet allows employees to access company resources through a secure, Internet-like interface, while an extranet extends this access to suppliers, customers, and other external agents.

Overall, the intersection of [[The Internet and Business]] has created a dynamic landscape where e-commerce thrives, requiring robust governance and innovative use of technology to meet the needs of users and organizations alike.

