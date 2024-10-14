---
tags:
- inti
- topic
- note
Class: "[[IT Infrastructure Class (INTI)]]"
Topic: "[[Network Security and Network Design]]"
---

# Cyber Threats

## Network Attacks
- **Packet Sniffing:** Attackers capture and analyze network traffic to obtain sensitive information like passwords or session tokens. Tools such as Wireshark are commonly used.
  
- **Man-in-the-Middle (MitM):** By intercepting communication between two parties, attackers can eavesdrop or manipulate the data being exchanged. For example, they could alter transaction details during an online banking session.

- **DNS Hacking:** Attackers manipulate DNS records to redirect users to malicious websites, often through phishing emails that trick users into entering credentials on fake sites.

- **Denial of Service (DoS) and Distributed Denial of Service (DDoS):** 
  - DoS attacks flood a server with excessive traffic, making it unable to respond to legitimate requests.
  - DDoS attacks use multiple compromised systems to launch a coordinated assault, amplifying the impact.

## Web Attacks
- **Phishing:** Attackers impersonate legitimate entities to trick users into revealing sensitive information. Phishing attacks can be executed through emails, text messages, or fake websites.

- **SQL Injection:** By injecting malicious SQL code into input fields (like login forms), attackers can manipulate databases to extract, modify, or delete data. This technique exploits the way applications handle user input.

- **Cross-Site Scripting (XSS):** Attackers inject malicious scripts into web pages viewed by users, enabling them to steal cookies or session tokens, leading to unauthorized access to user accounts.

## OS, Applications, and Software Attacks
- **Virus:** A self-replicating program that spreads by attaching itself to clean files and propagating throughout the system, often causing damage to files and data.

- **Trojan:** A malicious program that masquerades as legitimate software, enabling attackers to gain unauthorized access to systems.

- **Worms:** These malware replicate themselves to spread to other computers, often exploiting network vulnerabilities without needing human intervention.

- **Rootkits:** A set of software tools used to hide the presence of certain processes or programs from normal methods of detection, allowing continued access and control over a system.

- **Buffer Overflow:** Attackers exploit vulnerabilities in software that fail to properly handle data input, allowing them to execute arbitrary code or crash the system.

## Social Engineering
### Definition
- Social engineering involves manipulating individuals into revealing confidential information by exploiting psychological triggers and human behavior rather than relying solely on technical exploits.

### Examples of Social Engineering Attacks
- **Phishing:** Fraudulent emails prompt users to click on malicious links.
  
- **Pretexting:** The attacker creates a fabricated scenario to obtain information, such as posing as a tech support agent.

- **Baiting:** Attackers entice users to download malicious software by promising something appealing, like free software or access to restricted content.

### Protection Strategies
- **Education and Awareness:** Training users to recognize social engineering tactics and report suspicious activities.
- **Password Security:** Encouraging strong password practices and the use of two-factor authentication.

## Cyberwar: Stuxnet (2009)
### Overview of Stuxnet
- Stuxnet is a sophisticated computer worm believed to be developed by the U.S. and Israeli governments to target Iran's nuclear program. It represents a significant example of state-sponsored cyber warfare.

### How Stuxnet Works
- The worm spread via infected USB drives and exploited multiple zero-day vulnerabilities in Windows, allowing it to bypass traditional security measures.
- Stuxnet specifically targeted Siemens software used in industrial control systems, affecting thousands of machines.
- Upon infecting a system, Stuxnet checked for the presence of Siemens PCS7/STEP7 software and embedded itself into these environments.
- It replaced critical communication libraries, manipulating data exchanged with PLCs and altering the operation of industrial equipment.
- Stuxnet executed commands that resulted in the malfunction of centrifuges used in uranium enrichment, causing physical damage while providing false feedback to operators.

### Lessons Learned from Stuxnet
- **Sophistication of Attacks:** Stuxnet highlighted the potential for high-profile, government-sponsored malware, emphasizing the need for advanced security measures.
- **Defense-in-Depth:** Organizations should implement multiple layers of security controls to protect against sophisticated threats.
- **Awareness of Insider Threats:** Training employees to recognize social engineering tactics can help prevent breaches.
- **Regular Updates and Patch Management:** Keeping systems and software up to date is crucial in defending against known vulnerabilities.
