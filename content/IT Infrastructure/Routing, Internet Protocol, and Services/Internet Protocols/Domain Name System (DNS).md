---
tags: 
- inti
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Routing, Internet Protocol and Services]]"
---

# Domain Name System (DNS)

The **Domain Name System (DNS)** is a fundamental component of the Internet that translates human-readable domain names into machine-readable IP addresses. This translation process is crucial for enabling users to access websites without needing to remember complex numerical IP addresses.

## Structure of DNS

### Hierarchical Organization
- **Domain Hierarchy**: DNS is structured in a hierarchical manner, consisting of various levels:
  - **Top-Level Domains (TLDs)**: The highest level, such as .com, .org, .net, .edu, and country-specific domains like .uk and .jp.
  - **Second-Level Domains**: These are directly beneath TLDs, typically representing organizations or entities (e.g., google.com, wikipedia.org).
  - **Subdomains**: Additional divisions within second-level domains, allowing for further organization (e.g., mail.google.com, en.wikipedia.org).
  
### DNS Records
- DNS utilizes various record types to store information about domains:
  - **A Record**: Maps a domain name to its corresponding IPv4 address.
  - **AAAA Record**: Maps a domain name to its corresponding IPv6 address.
  - **CNAME Record**: Alias for a domain name, allowing one domain to point to another (e.g., www.example.com can point to example.com).
  - **MX Record**: Specifies mail exchange servers for the domain, directing email to the correct server.
  - **NS Record**: Indicates the authoritative name servers for a domain.

## DNS Resolution Process

The DNS resolution process is the series of steps that occur when a user attempts to access a website by entering its domain name into a browser. This process involves multiple components and can be summarized in several stages:

### 1. User Query
- **Initial Request**: When a user types a domain name into a web browser, the browser first checks its local cache to see if it already has the IP address stored.
- **Cache Check**: If the IP address is found in the cache, the browser uses it to connect to the server. If not, it proceeds to query a DNS server.

### 2. Recursive DNS Resolver
- **Resolver Function**: The query is sent to a **recursive DNS resolver**, typically managed by the user's Internet Service Provider (ISP). This resolver acts on behalf of the client and is responsible for resolving the domain name.
- **Cache Lookup**: The resolver first checks its own cache for the requested domain name.

### 3. Root DNS Servers
- **Root Query**: If the resolver cannot find the IP address in its cache, it sends a query to one of the **root DNS servers**. These servers are the highest level in the DNS hierarchy and do not store specific domain records but know where to direct queries.
- **Referral to TLD Servers**: The root server responds with a referral to the appropriate **TLD name servers** for the queried domain.

### 4. TLD Name Servers
- **TLD Query**: The resolver then queries the TLD name server for the domain. For example, if the domain is example.com, the resolver would contact the .com TLD server.
- **Referral to Authoritative Name Servers**: The TLD server responds with a referral to the **authoritative name servers** for the specific domain.

### 5. Authoritative Name Servers
- **Final Query**: The resolver queries the authoritative name server for the domain. This server contains the actual DNS records for the domain.
- **Response**: The authoritative server responds with the corresponding **A record** or **AAAA record**, providing the IP address for the requested domain.

### 6. IP Address Delivery
- **Return to Client**: The resolver receives the IP address from the authoritative server and caches it for future queries. It then returns the IP address to the user's browser.
- **Browser Connection**: The browser uses the received IP address to establish a connection to the web server, enabling the retrieval of the requested web page.

## Caching Mechanism
- **Local Caching**: To improve efficiency and reduce latency, DNS responses are cached at various levels (local browser cache, resolver cache, etc.). Caching reduces the need for repetitive queries to the DNS servers.
- **Time-To-Live (TTL)**: Each DNS record has a TTL value, which determines how long the record can be cached before it must be refreshed. TTL values can vary significantly based on the needs of the domain owner.

## Importance of DNS
- **User-Friendly Navigation**: DNS allows users to navigate the Internet easily using memorable domain names instead of complex IP addresses.
- **Decentralization**: The distributed nature of DNS enhances reliability and fault tolerance, ensuring that the system can withstand failures and continue to operate efficiently.
- **Load Distribution**: DNS can help distribute traffic load across multiple servers through techniques like **round-robin DNS**, where multiple IP addresses can be associated with a single domain name.

## Security Considerations
- **DNS Spoofing/Poisoning**: This is a malicious attack where incorrect DNS records are inserted into the cache, redirecting users to fraudulent sites.
- **DNSSEC**: To combat these attacks, **Domain Name System Security Extensions (DNSSEC)** add a layer of security by enabling DNS responses to be verified for authenticity, ensuring that users reach the legitimate sites they intend to visit.
- **DDoS Attacks**: DNS servers can be targeted in Distributed Denial of Service (DDoS) attacks, which can lead to service outages and disrupted access to websites.

## Conclusion
The **Domain Name System (DNS)** is an essential component of the Internet, facilitating the translation of human-friendly domain names into IP addresses. Understanding how DNS operates and the processes behind it is crucial for navigating the complexities of the Internet and ensuring secure and efficient access to online resources.