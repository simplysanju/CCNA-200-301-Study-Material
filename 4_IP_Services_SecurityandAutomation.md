# Week 4: IP Services, Security, and Automation

## Day 22: DHCP (Dynamic Host Configuration Protocol)

Concept: DHCP Process (DORA), Configuring a DHCP Server

DHCP (Dynamic Host Configuration Protocol) is a network service that dynamically assigns IP addresses to devices. Without DHCP, administrators would need to manually configure IP addresses for each device, which is inefficient in large networks.

**DHCP Process - DORA (Discover, Offer, Request, Acknowledge):**

1. **Discover:** A client broadcasts a request for an IP address.
2. **Offer:** The DHCP server responds with an available IP address.
3. **Request:** The client requests the offered IP.
4. **Acknowledge:** The server confirms the lease and assigns the IP.

**DHCP Configuration on a Cisco Router:**

```Router(config)# ip dhcp pool LAN```
```Router(dhcp-config)# network 192.168.1.0 255.255.255.0```
```Router(dhcp-config)# default-router 192.168.1.1```
```Router(dhcp-config)# dns-server 8.8.8.8```
```Router(dhcp-config)# exit```
```Router(config)# ip dhcp excluded-address 192.168.1.1 192.168.1.10```

**Activity:** Set up DHCP on a Cisco router in Packet Tracer and verify leases using ```show ip dhcp binding.```

## Day 23: DNS (Domain Name System)

Concept: DNS Hierarchy, Resolving Names to IPs

DNS (Domain Name System) is a hierarchical service that translates human-readable domain names (e.g., google.com) into IP addresses. This allows users to access websites without memorizing numerical addresses.

**DNS Hierarchy:**

1. Root Servers: The top-level servers that direct queries to TLD (Top-Level Domain) servers.
2. TLD Servers: Handle domain extensions like .com, .org, .edu.
3. Authoritative DNS Servers: Store domain name records and respond with IP addresses.
4. Recursive Resolvers: Forward DNS queries to the appropriate server and return the response to the client.

**Using DNS Query Tools:**

```nslookup google.com (Windows/Linux)```
```dig google.com (Linux)```

**Activity:** Use ```nslookup``` or ```dig``` to query DNS records and analyze responses.

## Day 24: Security Fundamentals

Concept: Threats (e.g., DoS), ACLs (Access Control Lists), Best Practices

Network security involves protecting infrastructure against cyber threats like Denial-of-Service (DoS) attacks, unauthorized access, and malware.

**Common Network Security Threats:**

- DoS/DDoS Attacks: Overloading a network to cause service disruption.
- Phishing & Social Engineering: Tricking users into revealing credentials.
- Man-in-the-Middle (MITM) Attacks: Intercepting network communication.

**Access Control Lists (ACLs):**

ACLs filter network traffic based on defined rules.

Example of a standard ACL to block a specific host:

```Router(config)# access-list 10 deny 192.168.1.100```
```Router(config)# access-list 10 permit any```
```Router(config)# interface fa0/0```
```Router(config-if)# ip access-group 10 in```

Activity: Configure a **standard ACL** in Packet Tracer to restrict access to a specific subnet.

## Day 25: VPNs and Wireless Security

Concept: VPN Types (Site-to-Site, Remote), WPA2/WPA3 for Wi-Fi

A Virtual Private Network (VPN) provides a secure connection over an untrusted network (e.g., the Internet) by encrypting data traffic.

**Types of VPNs:**

- Site-to-Site VPN: Connects entire networks securely (e.g., two offices).
- Remote Access VPN: Allows individual users to securely connect to the network from anywhere.

**Wi-Fi Security (WPA2 & WPA3):**

- WPA2 (Wi-Fi Protected Access 2): Uses AES encryption for security.
- WPA3: Introduces stronger encryption and protection against brute-force attacks.

**Activity:** Research VPN setup and simulate **WPA3 configuration** in Packet Tracer.

## Day 26: Automation and Programmability

Concept: SDN (Software-Defined Networking), APIs, Cisco DNA

Traditional networks rely on manual configuration, but network automation enables dynamic control of devices using Software-Defined Networking (SDN) and APIs.

**Key Concepts in Network Automation:**

- SDN (Software-Defined Networking): Centralized control plane for network traffic.
- APIs (Application Programming Interfaces): Used to manage devices programmatically.
- Cisco DNA (Digital Network Architecture): Provides AI-driven automation for large-scale networks.

**Activity:** Watch a **Cisco DNA Center demo** and read about **REST APIs** for network automation.

## Day 27: Network Management Protocols

Concept: SNMP, Syslog, NTP (Network Time Protocol)

Proper network management is essential for monitoring performance and diagnosing issues.

**Common Network Management Protocols:**
- SNMP (Simple Network Management Protocol): Monitors network devices.
- Syslog: Centralized logging system for tracking network events.
- NTP (Network Time Protocol): Synchronizes time across devices.

**Configuring NTP on a Cisco Router:**

```Router(config)# ntp server 192.168.1.100```
```Router(config)# clock timezone UTC 0```

**Activity:** Configure **NTP on a router** and verify time synchronization.**

## Day 28: Final Review

Concept: Revisit Weak Areas (e.g., Subnetting, OSPF)

Before the exam, it's crucial to reinforce weak areas such as subnetting, routing protocols (OSPF, static routes), NAT, and VLANs.

**Common Exam Topics to Review:**

- Subnetting and IP Addressing.
- Static vs. Dynamic Routing.
- VLANs and Inter-VLAN Routing.
- DHCP, DNS, and NAT.
- Network Security (ACLs, VPNs).

**Activity:** Take a **Cisco practice exam** and review incorrect answers.

## Day 29: Hands-On Practice

Concept: End-to-End Network Setup

Practical experience is essential for real-world networking.

**Lab Setup (Packet Tracer):**

- Design a multi-router network.
- Implement VLANs with inter-VLAN routing.
- Configure DHCP, NAT, and OSPF.
- Troubleshoot using ping, show ip route, and debug commands.

**Activity:** Build a complete **network with VLANs, routing, NAT, and DHCP in Packet Tracer.**

## Day 30: Exam Prep

Concept: Full Exam Simulation

The final step is to take a **full-length CCNA practice test** and refine your exam strategy.

**Tips for Exam Day:**

- Manage Time: Allocate time per question (~1.5 min per question).
- Use the CLI: In the real CCNA exam, use CLI to verify answers.
- Practice Subnetting: Speed is key in subnetting calculations.

**Activity:** Take a **full-length CCNA 200-301 practice test** and review all **incorrect answers** to strengthen weak areas.