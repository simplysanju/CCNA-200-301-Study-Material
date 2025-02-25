# Week 1: Network Fundamentals

Goal: Build a strong foundation in networking basics.

## Day 1: Introduction to Networking

**Concept**

A network is a collection of interconnected devices (computers, servers, printers, etc.) that communicate with each other to share resources and data. Networks can be categorized based on their size and purpose:

- **LAN (Local Area Network)**: A network within a small geographic area, such as a home, office, or building. Example: A Wi-Fi network in your home.

- **WAN (Wide Area Network)**: A network that spans large geographic areas, often connecting multiple LANs. Example: The internet.

- **MAN (Metropolitan Area Network)**: A network that covers a city or campus. Example: A university network.

**Network Topologies** define the arrangement of devices in a network:

**Star Topology:** All devices connect to a central hub or switch. Example: Home Wi-Fi networks.

**Bus Topology:** Devices are connected to a single communication line (bus). Example: Early Ethernet networks.

**Ring Topology:** Devices are connected in a circular fashion. Example: Token Ring networks.

**Activity**

**Read:** Study networking basics from Cisco’s official CCNA guide or free online articles.
**Watch:** A beginner-friendly video on networking fundamentals (e.g., Cisco’s CCNA intro on YouTube).

**Resource**
Cisco’s official CCNA study guide or free online articles.

## Day 2: OSI and TCP/IP Models

**Concept**

The **OSI (Open Systems Interconnection) model** is a 7-layer framework that standardizes network communication:

1. Physical Layer (Layer 1): Deals with physical connections (cables, switches).

2. Data Link Layer (Layer 2): Handles MAC addressing and framing.

3. Network Layer (Layer 3): Manages IP addressing and routing.

4. Transport Layer (Layer 4): Ensures reliable data transfer (TCP/UDP).

5. Session Layer (Layer 5): Manages sessions between applications.

6. Presentation Layer (Layer 6): Handles data formatting and encryption.

7. Application Layer (Layer 7): Provides network services to applications.

The **TCP/IP model** is a simplified 4-layer model:

1. Network Access Layer: Combines OSI Layers 1 and 2.

2. Internet Layer: Corresponds to OSI Layer 3.

3. Transport Layer: Corresponds to OSI Layer 4.

4. Application Layer: Combines OSI Layers 5, 6, and 7.

**Activity**
- Memorize: Learn the layers and their functions.
- Draw: Create a comparison chart between the OSI and TCP/IP models.

**Tip**
Focus on Layer 1 (Physical), Layer 2 (Data Link), and Layer 3 (Network) as they are foundational for networking.

## Day 3: Network Devices

**Concept**

Network devices are hardware components that facilitate communication in a network:

**Hub:** A basic device that connects multiple devices in a LAN. It broadcasts data to all connected devices.

**Switch:** A smarter device that forwards data only to the intended recipient using MAC addresses.

**Router:** Connects different networks (e.g., LAN to WAN) and routes data based on IP addresses.

**Access Point (AP):** Provides wireless connectivity to devices.

**Firewall:** Protects the network by filtering incoming and outgoing traffic based on security rules.

**Activity**

- Research: Study the functions of each device.
- Watch: A demo video comparing switches and routers.

## Day 4: IP Addressing Basics (IPv4)

**Concept**

An **IP address** is a unique identifier assigned to each device on a network. IPv4 addresses are 32-bit numbers written in dotted-decimal notation (e.g., 192.168.1.1). Key concepts:

- Binary to Decimal Conversion: IPv4 addresses are binary numbers converted to decimal for readability.
- IP Classes: IPv4 addresses are divided into classes:
* Class A: 1.0.0.0 to 126.0.0.0 (large networks).
* Class B: 128.0.0.0 to 191.255.0.0 (medium networks).
* Class C: 192.0.0.0 to 223.255.255.0 (small networks).
- Public vs. Private IPs: Public IPs are routable on the internet, while private IPs are used within local networks.

**Activity**

- Practice: Convert binary numbers to decimal.
- Identify: Determine the class of given IP addresses.

## Day 5: Subnetting Part 1

**Concept**

**Subnetting** divides a network into smaller subnetworks (subnets) to improve efficiency and security. Key terms:

**Subnet Mask:** A 32-bit number that defines the network and host portions of an IP address (e.g., 255.255.255.0).

**CIDR Notation:** A shorthand for subnet masks (e.g., /24 means 24 bits are used for the network portion).

**Activity**
**Solve:** Subnet a /24 network into 4 smaller subnets.

## Day 6: Subnetting Part 2

**Concept**

Advanced subnetting involves:

**Finding Hosts per Subnet:** Calculate the number of usable IPs in a subnet.

**Usable IPs:** Subtract 2 from the total hosts (one for the network ID and one for the broadcast address).

**Activity**
- Practice: Solve 10 subnetting problems with varying CIDR notations.

## Day 7: IPv6 Basics

**Concept**

IPv6 is the successor to IPv4, designed to address the exhaustion of IPv4 addresses. Key features:

**128-bit Addresses:** Written in hexadecimal (e.g., 2001:0db8:85a3::8a2e:0370:7334).

**Address Types:**

- Unicast: One-to-one communication.
- Multicast: One-to-many communication.
- Anycast: One-to-nearest communication.

**Importance:** IPv6 provides a larger address space and improved security.

**Activity**
- Compare: IPv4 vs. IPv6.
- Write: Create an example IPv6 address.

This structured and detailed approach ensures a thorough understanding of Network Fundamentals, aligning with the CCNA curriculum. Each day’s content is designed to build knowledge progressively, with practical activities to reinforce learning.
