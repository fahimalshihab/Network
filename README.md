# Network

# What Is a Computer Network?
A computer network is a system that connects two or more computing devices for transmitting and sharing information. Computing devices include everything from a mobile phone to a server. These devices are connected using physical wires such as fiber optics, but they can also be wireless.

# Key Components of a Computer Network

From a broader lens, a computer network is built with two basic blocks: nodes or network devices and links. The links connect two or more nodes with each other.

![image](https://github.com/fahimalshihab/Network/assets/97816146/5cb0a2c9-5dde-43d5-8b85-244ff8a83a0d)

## 1. Network Devices
Network devices or nodes are computing devices that need to be linked in the network. Some network devices include:

* **End Devices:** Laptops, phones, tablets - what users interact with directly.
* **Servers:** Store data and run programs for other devices on the network.
* **Routers:** Direct data packets to their final destinations across networks.
* **Switches:** Connect multiple devices within a single network segment.
* **Gateways:** Act as passage points between different networks, often combining router and firewall functionalities. 

## 2. Links
Links are the transmission media which can be of two types:

* **Wired:** Physical cables that directly connect devices, like dedicated lanes on a highway. Examples include coaxial cables, phone lines, twisted-pair cables (Ethernet), and fiber optic cables.
* **Wireless:** No cables needed! These links use radio waves or other electromagnetic signals to send data through the air, similar to signals reaching a wide area. Common examples include Wi-Fi, cellular networks, communication satellites, and spread spectrum technology (used in Wi-Fi and Bluetooth).

## 3. Communication protocols
A communication protocol is a set of rules followed by all nodes involved in the information transfer.TCP/IP is a conceptual model that standardizes communication in a modern network. It suggests four functional layers of these communication links:

* **Network Access Layer:** Deals with the physical transmission of data (cables, fibers).
* **Internet Layer:** Packages data into packets for sending and receiving.
* **Transport Layer:** Ensures reliable connections between devices.
* **Application Layer:** Defines how programs access the network for data transfer.

## 4. Network Defense
Network defenses are essential for protecting data on a network.
Common tools include firewalls, intrusion detection, access control, and anti-DDoS measures.

# Types of Computer Networks

Computer networks can be classified based on several criteria, including:

* **Transmission medium:** wired vs. wireless
* **Network size:** geographical scale
* **Topology:** network layout
* **Organizational intent:** purpose of the network

#### Here's a breakdown of different network types based on geographical scale:

**Nanoscale networks:** Facilitate communication between tiny sensors and actuators.

**Personal Area Network (PAN):** Connects devices used by a single person, like laptops, printers, etc.

**Local Area Network (LAN):** Connects devices within a limited area (schools, offices, buildings).

**Storage Area Network (SAN):** Dedicated network for block-level data storage (disk arrays, tape libraries).

**Campus Area Network (CAN):** Collection of interconnected LANs used by universities or governments.

**Metropolitan Area Network (MAN):** Spans across a city.

**Wide Area Network (WAN):** Covers large geographical areas (states, countries).

**Enterprise Private Network (EPN):** Single network for large organizations to connect offices.

**Virtual Private Network (VPN):** Secure overlay network on top of a public network.

**Cloud Network:** WAN with infrastructure delivered via cloud services.

#### Based on organizational intent, networks can be classified as:

**Intranet:** Secure network controlled by a single entity (internal users only).

**Internet:** Global network connecting governments, businesses, individuals, etc.

**Extranet:** Similar to intranet, but with controlled access for external partners/customers.

**Darknet:** Overlay network on the internet, accessible only through specialized software.


# Identifying Devices on a Network

Every device connected to a network has two unique identifiers:

* **IP Address:** This is a logical address assigned to a device for communication within the network. It can be temporary (DHCP) or permanent (static). Think of it as a house number on a street.

* **MAC Address:** This is a unique hardware address burned into the device's network interface card (NIC). It's permanent and globally unique, acting like a fingerprint for the device.

## IP Addresses

An IP address identifies a device on a network. It's a set of four numbers separated by dots (e.g., 192.168.1.77). 

* **Types:**
    * **Public IP:** Identifies a device on the internet. Think of it as a public street address.
    * **Private IP:** Identifies a device within a local network (e.g., home or office). Think of it as a private apartment number within a building.

* **Uniqueness:**
    * A public IP is unique to a device on the internet at a given time.
    * A private IP can be reused on different networks.
  ![image](https://github.com/fahimalshihab/Network/assets/97816146/e6624cb2-61f6-4cda-89d5-87283c33bffc)

These two devices will be able to use their private IP addresses to communicate with each other. However, any data sent to the Internet from either of these devices will be identified by the same public IP address. Public IP addresses are given by your Internet Service Provider (or ISP) at a monthly fee (your bill!)

![image](https://github.com/fahimalshihab/Network/assets/97816146/e955a199-2f66-4108-9ec1-ad6249960d00)


## IP addresses come in two versions: IPv4 and IPv6.

* **IPv4:** The current dominant protocol, using 32-bit numbers (limited to around 4.3 billion addresses). Imagine it like a small town running out of street names.

* **IPv6:** The next-generation protocol, using 128-bit numbers (340 trillion-plus). Think of it as a giant city with plenty of unique addresses.

**Benefits of IPv6:**

* **Solves address shortage:** Provides enough addresses for the ever-growing internet.
* **More efficient:** Uses improved methods for routing data packets.

  ![image](https://github.com/fahimalshihab/Network/assets/97816146/b72a99ad-6561-4851-a1bf-338e8f1a0e77)

## MAC Addresses

Every network device has a unique identifier called a Media Access Control (MAC) address. It's a 12-character hexadecimal number (0-9 and A-F) burned into the network interface card (NIC) during manufacturing.

* **Format:** XX:XX:XX:XX:XX:XX (separated by colons)
* **Uniqueness:** Permanent and globally unique, like a device fingerprint.
* **Structure:**
    * First 6 characters: Identify the NIC manufacturer
    * Last 6 characters: Unique identifier assigned by the manufacturer

**Example:** a4:c3:f0:85:ac:2d
![image](https://github.com/fahimalshihab/Network/assets/97816146/560103f2-47fe-4f35-8fd8-d82553bf44cd)


# Ping

Ping is a network tool that uses ICMP (Internet Control Message Protocol) packets to test a connection's existence and performance. It sends an "echo request" and waits for an "echo reply" from the target device.

* **Measures:** Round-trip time (RTT) of ICMP packets, indicating connection speed and reliability.
* **Targets:** Devices on your network or websites.
* **Usage:** Simple to use, pre-installed on most operating systems (e.g., Linux, Windows).
* **Syntax:** `ping <IP address or website URL>`

  ![image](https://github.com/fahimalshihab/Network/assets/97816146/5b73b137-cca7-4758-af58-352c3eb706c6)

# Local Area Network (LAN) Topologies
Over the years, there has been experimentation and implementation of various network designs. In reference to networking, when we refer to the term "topology", we are actually referring to the design or look of the network at hand. Let's discuss the advantages and disadvantages of these topologies below.
![image](https://github.com/fahimalshihab/Network/assets/97816146/e6e611ac-89bc-4ad1-9f74-478a8d996416)


**Star Topology:**

* **Most common:** Devices connect individually to a central switch/hub.
* **Advantages:**
    * Scalable: Easy to add/remove devices.
    * Reliable: Failure of one device doesn't affect others.
* **Disadvantages:**
    * Costly: Requires more cables and central device.
    * Central device failure disrupts the entire network.
![image](https://github.com/fahimalshihab/Network/assets/97816146/ed6b555a-720e-4bea-bf25-8909338e1554)


**Bus Topology:**

* **Simple and cost-effective:** Devices connect to a single backbone cable.
* **Advantages:**
    * Easy to set up: Requires minimal cabling and equipment.
* **Disadvantages:**
    * Prone to bottlenecks: All devices share the same bandwidth.
    * Difficult to troubleshoot: Issues can arise from any device on the bus.
    * Single point of failure: Backbone cable failure disables the entire network.
![image](https://github.com/fahimalshihab/Network/assets/97816146/4067b1bd-38e5-47b1-9801-8580473be352)

**Ring Topology:**

* **Devices form a closed loop:** Data travels in one direction, passing through each device.
* **Advantages:**
    * Easy to troubleshoot: Fault isolation is simpler.
    * Less prone to bottlenecks: Traffic is more controlled.
* **Disadvantages:**
    * Slower performance: Data may need to travel through multiple devices.
    * Single point of failure: A break in the loop or device failure disrupts the network.
 
# What is a Switch?
Switches are dedicated devices within a network that are designed to aggregate multiple other devices such as computers, printers, or any other networking-capable device using ethernet. These various devices plug into a switch's port. Switches are usually found in larger networks such as businesses, schools, or similar-sized networks, where there are many devices to connect to the network. Switches can connect a large number of devices by having ports of 4, 8, 16, 24, 32, and 64 for devices to plug into.

Switches are much more efficient than their lesser counterpart (hubs/repeaters). Switches keep track of what device is connected to which port. This way, when they receive a packet, instead of repeating that packet to every port like a hub would do, it just sends it to the intended target, thus reducing network traffic.
![image](https://github.com/fahimalshihab/Network/assets/97816146/1a7cea1e-55eb-4704-9951-a3f468554b0a)

Both Switches and Routers can be connected to one another. The ability to do this increases the redundancy (the reliability) of a network by adding multiple paths for data to take. If one path goes down, another can be used. Whilst this may reduce the overall performance of a network because packets have to take longer to travel, there is no downtime -- a small price to pay considering the alternative.

# What is a Router?
It's a router's job to connect networks and pass data between them. It does this by using routing (hence the name router!).

Routing is the label given to the process of data travelling across networks. Routing involves creating a path between networks so that this data can be successfully delivered.

# Subnetting

Subnetting is the process of dividing a large network (like a /16 IP address block) into smaller, more manageable networks (subnets). It's like subdividing a large apartment complex into smaller buildings, each with its own set of addresses.

**Benefits of Subnetting:**

* **Improved network efficiency:** Allocate IP addresses more efficiently to specific network segments.
* **Enhanced security:** Isolate network traffic and improve control by creating separate subnets for different departments or functions.
* **Scalability:** Makes it easier to add new devices to the network without needing to redesign the entire addressing scheme.

**How Subnetting Works:**

Subnetting borrows bits from the host portion of an IP address to create subnets. This is done using a subnet mask, which defines the network portion of the address.

**Example:**

* Original network: 192.168.1.0/16 (has 65,536 potential addresses)
* Subnet mask: 255.255.255.128 (/25) (creates two subnets)
* Subnet 1: 192.168.1.0/25 (usable addresses: 192.168.1.1 - 192.168.1.126)
* Subnet 2: 192.168.1.128/25 (usable addresses: 192.168.1.129 - 192.168.1.254)


Routing is useful when devices are connected by many paths, such as in the example diagram below.

![image](https://github.com/fahimalshihab/Network/assets/97816146/6292b1fa-34e3-4dfb-a6b8-5cc34a17e32f)

# The ARP Protocol


Recalling from our previous tasks that devices can have two identifiers: A MAC address and an IP address, the Address Resolution Protocol or ARP for short, is the technology that is responsible for allowing devices to identify themselves on a network.

Simply, the ARP protocol allows a device to associate its MAC address with an IP address on the network. Each device on a network will keep a log of the MAC addresses associated with other devices.

When devices wish to communicate with another, they will send a broadcast to the entire network searching for the specific device. Devices can use the ARP protocol to find the MAC address (and therefore the physical identifier) of a device for communication.
![image](https://github.com/fahimalshihab/Network/assets/97816146/41e030cf-adf9-4413-a290-231fea02f938)


## How ARP Works

ARP (Address Resolution Protocol) helps translate IP addresses (logical addresses) to MAC addresses (physical addresses) on a network. Devices maintain a cache to store these mappings for faster communication.

**The Process:**

1. **Device Needs an IP Address:** A device wants to send data to another device on the network using an IP address.
2. **ARP Request Broadcast:** The device broadcasts an ARP request message on the network.
3. **Matching Device Responds:** If a device on the network has the matching IP address, it replies with an ARP response message containing its MAC address.
4. **Cache Update:** The requesting device receives the reply and stores the IP-to-MAC address mapping in its ARP cache for future reference.

**ARP Messages:**

* **ARP Request:** Broadcasted message asking "Who has this IP address?"
* **ARP Reply:** Response message containing the corresponding MAC address.

**Benefits of ARP:**

* **Efficient Communication:** Enables devices to communicate by translating IP addresses to physical addresses.
* **Dynamic Caching:** ARP caches are updated automatically, adapting to network changes.
# The DHCP Protocol
IP addresses can be assigned either manually, by entering them physically into a device, or automatically and most commonly by using a DHCP (Dynamic Host Configuration Protocol) server. When a device connects to a network, if it has not already been manually assigned an IP address, it sends out a request (DHCP Discover) to see if any DHCP servers are on the network. The DHCP server then replies back with an IP address the device could use (DHCP Offer). The device then sends a reply confirming it wants the offered IP Address (DHCP Request), and then lastly, the DHCP server sends a reply acknowledging this has been completed, and the device can start using the IP Address (DHCP ACK).

![image](https://github.com/fahimalshihab/Network/assets/97816146/61c67e9b-ac94-4aa3-af50-97f36646d74b)

## OSI Model (Open Systems Interconnection)

The OSI model is a conceptual framework that defines how network communication occurs between devices. It consists of seven layers, each with specific functionalities:

![image](https://github.com/fahimalshihab/Network/assets/97816146/cf831b18-d9d5-4a8d-8280-8e2316b6b679)


**7. Application Layer:**

* **Function:** Provides network services directly to end-user applications.
* **Examples:** Web browsing (HTTP), file transfer (FTP), email (SMTP, POP), Domain Name System (DNS).

**6. Presentation Layer:**

* **Function:** Prepares data for the application layer by handling formatting, encryption, and compression.
* **Tasks:** Ensures data is presented in a compatible format for receiving applications.

**5. Session Layer:**

* **Function:** Establishes, manages, and terminates communication sessions between devices.
* **Tasks:** Sets up connections, ensures data exchange, and closes sessions after data transfer.

**4. Transport Layer:**

* **Function:** Provides reliable data transfer by breaking data into segments, handling errors, and ensuring order of delivery.
* **Tasks:** Segments data for efficient transmission, reassembles segments at the receiver, implements flow control to manage data rate, and error control to verify data integrity.

**3. Network Layer:**

* **Function:** Routes data packets across networks based on IP addresses.
* **Tasks:** Breaks data from the transport layer into packets, adds routing information for network traversal, and reassembles packets at the destination. 

**2. Data Link Layer:**

* **Function:** Transmits data frames over the physical network medium.
* **Sublayers:**
    * Logical Link Control (LLC): Manages protocols, error checking, and frame synchronization.
    * Media Access Control (MAC): Identifies devices on the network using MAC addresses and controls access to the physical medium.

**1. Physical Layer:**

* **Function:** Establishes the physical connection between network devices.
* **Examples:** Ethernet cables, Wi-Fi signals, fiber optic cables.

**Benefits of OSI Model:**

* Standardization: Enables communication between devices from different vendors.
* Modular Design: Simplifies troubleshooting by isolating issues within specific layers.


**Encapsulation:**

As data travels through the OSI layers, it undergoes encapsulation. Each layer adds a header containing information relevant to its function. This header is like an envelope containing the actual data and instructions for the next layer.


# TCP/IP Model

The TCP/IP model is a four-layer (sometimes described as five) suite of protocols defining data transmission over networks like the internet. It offers a simpler and more practical approach compared to the OSI model.

**Layers:**

1. **Network Access Layer (sometimes combined with Data Link Layer):**
   * Handles physical network connections and Media Access Control (MAC addresses).
   * Examples: Ethernet, Wi-Fi.

2. **Internet Layer:**
   * Routes data packets across networks using IP addresses.
   * Protocol: IP (Internet Protocol)

3. **Transport Layer:**
   * Provides reliable data transfer between applications.
   * Protocols: TCP (Transmission Control Protocol) and UDP (User Datagram Protocol).
     * TCP: Guarantees in-order delivery with error checking and retransmission (reliable).
     * UDP: Faster but connectionless, suitable for real-time applications (e.g., streaming) (unreliable).

4. **Application Layer:**
   * Provides network services to applications.
   * Examples: HTTP (web browsing), FTP (file transfer), SMTP (email), DNS (domain name system).

**Benefits of TCP/IP Model:**

* **Simple and Efficient:** Focuses on practical network communication.
* **Flexible and Adaptable:** Accommodates diverse network technologies.
* **Vendor-Independent:** Enables communication between devices from different vendors.

![tt6b2sau1mdcg73qt4iz](https://github.com/fahimalshihab/Network/assets/97816146/350f49d2-7716-482d-b794-71b0385c6719)

# Differences between IPv4 and IPv6

## IPv4 in a Nutshell

* Introduced in 1981, the first widely used internet protocol version.
* 32-bit address (e.g., 192.168.1.1).
* Limited addresses, nearing exhaustion.
* No built-in security, vulnerable to attacks.
* Gradually being replaced by the more secure IPv6 with a much larger address space.
![image](https://github.com/fahimalshihab/Network/assets/97816146/0dd7f6fe-24ff-4644-8b15-f1792ebfb2bc)

## IPv6 in a Nutshell

* Successor to IPv4, designed to address limitations.
* 128-bit address (written as 8 hex groups: e.g., 2001:db8::1).
* Vastly larger address space, solving exhaustion issues.
* Built-in security features for better protection.
* Transition from IPv4 ongoing, both still in use.
![image](https://github.com/fahimalshihab/Network/assets/97816146/14377764-7db9-47c2-b406-6dbe7f2f9671)

## Benefits of IPv6

IPv6, the next generation of the Internet Protocol, offers several advantages over IPv4:

* **Larger Address Space:** IPv6 boasts a significantly larger address space compared to IPv4. This vast space can accommodate the ever-increasing number of internet-connected devices, a limitation faced by IPv4.
* **Enhanced Security:** Built-in security features are a core benefit of IPv6. These features help protect against attacks like spoofing, leading to more secure connections.
* **Improved Efficiency:**  A simpler header format in IPv6 allows for faster data transfer compared to the more complex header of IPv4.
* **Better Mobility:**  IPv6 is designed with mobile devices in mind, offering improved support for their specific connection needs.
* **Quality of Service (QoS):** Stronger support for QoS features enables better traffic management in IPv6. This can potentially improve audio and video quality on websites.
![image](https://github.com/fahimalshihab/Network/assets/97816146/6614195c-a13a-4877-99be-1c7d2d54f8b9)

# Network Discovery 

Network discovery is the process of identifying and locating devices on a network. It's essential for network administrators to:

* **Map the network:**  Visually represent the network topology (devices & connections).
* **Maintain inventory:**  Track devices (types, IP addresses).
* **Enforce access policies:**  Control device access to network resources.
* **Troubleshoot issues:**  Identify root causes of network problems (outages, security threats).

**Benefits:**

* Improved visibility into the network
* Streamlined network management
* Enhanced security posture
* Efficient troubleshooting

**How it Works:**

Network discovery tools leverage various protocols to find devices:

* **Ping Sweeps:** Sending ICMP echo requests to identify active devices.
* **IP Scans:** Systematically checking IP address ranges for responses.
* **SNMP (Simple Network Management Protocol):**  Collecting information from SNMP-enabled devices.
* **LLDP (Link Layer Discovery Protocol):**  Discovering neighboring devices through direct connections.

**Network Discovery Tools:**

These tools automate discovery, saving time and effort. They offer features like:

* **Automatic device mapping:** Creates visual network maps.
* **Performance monitoring:** Tracks device health and performance metrics.
* **QoE monitoring:** Analyzes user experience based on network performance.
* **Hardware health insights:** Provides information on hardware components (temperature, power supply).
* **Centralized dashboards:** Offers a single view of all discovered devices and details.

**Types of Discovered Devices:**

* Network devices (switches, routers, firewalls)
* Servers
* Printers
* Virtual machines
* Software applications

**Network Discovery Protocols:**

* **SNMP:**  The most common protocol for collecting device information.
* **LLDP:**  Enables neighboring devices to share information.
* **Ping:**  A simple tool to check if a device is active.

# Nmap
## What is Nmap?

Nmap (Network Mapper) is a free and open-source network discovery and security auditing tool. It's widely used for tasks like:

* Identifying active hosts on a network
* Discovering open ports and services
* Detecting operating systems (OS) running on devices
* Scanning for vulnerabilities

Nmap works by sending specially crafted packets to target hosts and analyzing the responses to gather information.

**Who uses Nmap?**

* **Network administrators:** Monitor host uptime, manage service updates, and create network inventory.
* **Security professionals:** Map network architecture, identify vulnerabilities, and support penetration testing.

**Zenmap: Graphical User Interface (GUI)**

Zenmap provides a user-friendly interface to visualize and interact with Nmap scan results. It offers features like:

* Different views for scan data
* Filtering options
* Graphing capabilities

**Basic Nmap Syntax**

nmap <Scan Type(s)><Options> <target specification>


* **Scan Types:** Specify the type of scan to perform (e.g., TCP connect scan, SYN scan, etc.)
* **Options:** Customize your scan with various options (e.g., port range, aggressive scan, OS detection)
* **Target Specification:** Define the target(s) to scan using IP addresses, hostnames, or CIDR notation

**Example Scan:**

nmap 192.168.108.129  # Simple scan of target IP


**Nmap Scripting Engine (NSE)**

NSE extends Nmap's functionality by enabling scripts for:

* Brute-force attacks
* Vulnerability discovery
* Exploitation

**NSE Script Categories:**

* **Script Execution Time:**
    * prerule (before scan)
    * host (during scan)
    * service (after scanning a host)
    * postrule (after entire scan)
* **Script Goals and Safety:**
    * Broadcast
    * Authentication
    * Default
    * Malware
    * Discovery
    * Brute force
    * DOS
    * Fuzzer
    * Exploit

**Running NSE Scripts:**

* `-sC`: Executes all default NSE scripts

**Examples:**

nmap -sC sample.com  # Run all default scripts on a host

nmap --script smb-os-discovery --script-trace sample.com  # Run specific script with tracing


**Nmap Integration**

Nmap integrates with other security tools like Metasploit Framework, enhancing penetration testing and security assessments.

**Platforms:**

Nmap is cross-platform compatible and runs on Linux, Windows, macOS, and other Unix-like systems.

**History and Development**

* First released in 1997 as a command-line tool
* Regular updates and new features
* Active community of users and developers

Nmap is a powerful tool for network security and remains a valuable asset for various network-related tasks.

# Cybersecurity Fingerprinting: Concept, Insights and Strategies
**What is cybersecurity fingerprinting?**

* It's a technique to gather information about a system or network by analyzing its unique characteristics.  {fingerprint}
* This information helps identify the system type, software, and potential vulnerabilities.

**Different fingerprinting techniques:**

* **Active fingerprinting:** Directly interacts with the target system to gather information. {playwright}
* **Passive fingerprinting:** Analyzes network traffic without interacting with the target system. {eye}
* **Hybrid fingerprinting:** Combines both active and passive techniques for a more comprehensive view. {yin-yang}

**Benefits of fingerprinting:**

* Helps detect threats and vulnerabilities. {shield}
* Aids in user authentication. {key}
* Provides valuable data for network mapping and security measures. {hammer}

**Important fingerprinting tools:**

* **Nmap:** Popular tool for active fingerprinting. {hammer}
* **p0f:** Focuses on passive fingerprinting by analyzing network traffic. {eye}
* **XProbe2:** Known for its versatility and accuracy in active fingerprinting. {hammer}

**Legal and ethical considerations:**

* User privacy and consent are crucial. {lock}
* Fingerprinting data needs to be collected and used responsibly. {balance-scale}

**The future of fingerprinting:**

* Advancements in AI and machine learning will enhance fingerprinting techniques. {brain}
* Continuous adaptation is necessary to keep pace with evolving threats. {recycle}

**Overall, cybersecurity fingerprinting is a valuable tool for defense against cyberattacks. By understanding its applications and limitations, security professionals can leverage it effectively.**


## Why Test a Network?

**Unveiling Network Weaknesses for Enhanced Security**

[shield] Businesses rely on robust networks to function efficiently. However, these networks are susceptible to cyberattacks due to the numerous software applications and devices they interact with. Vulnerabilities arise when weaknesses exist within the network, creating potential entry points for malicious actors. These weaknesses can lurk in various areas, including:

* Servers
* Firewalls
* Routers
* Modems
* Physical connection ports
* Operating systems
* Outdated software

Any of these vulnerabilities can be exploited by cybercriminals to gain unauthorized access to a network and inflict damage on critical business systems.

**Network Security Threats: A Multifaceted Landscape**

The ever-evolving threat landscape necessitates a comprehensive approach to network security. Network vulnerabilities can be exploited through a variety of malicious tactics, including:

* **Malware:** Malicious software designed to disrupt, damage, or steal data.**Active Directory: What and Why**

Active Directory (AD) is a Microsoft technology that helps organizations manage and organize their computer systems, users, and resources. It acts like a digital directory or address book for a network, keeping track of information about users, computers, and other networked devices.

**Key Purposes and Benefits of Active Directory**

* **Centralized Management**: All network resources can be managed and controlled in an organized and centralized manner with the help of Active Directory. Computers, printers, user accounts, and other networked equipment fall under this category.
* **User Authentication and Authorization**: It functions as a central authentication system, enabling users to log in with just their username and password and granting access according to their roles and permissions on the network.
* **Security**: Active Directory enables the implementation of security policies and access controls. To ensure that only authorized users have access to particular resources, administrators can establish and enforce security settings.
* **Group Policy**: Group Policy allows network administrators to apply and enforce settings on several computers at once. This helps in keeping software installations, security settings, and configurations consistent.
* **Resource Management**: It enables network resources like printers, files, and apps to be arranged and managed in an organized way. This makes it easier for administrators to allocate resources efficiently.
* **Scalability**: The increase in the size of the organization will not affect the functionality of Active Directory. The directory structure can readily accommodate more users, computers, and resources as the organization expands.
* **Single sign-on**: Users can utilize a single set of credentials to access a variety of resources and services while using Active Directory. This improves user convenience and streamlines the login procedure.

**Main Terminologies and Components of Active Directory**

* **Objects**: Resources that are present in the AD network are known as objects in Active Directory (AD). These resources include users, PCs, printers, contacts for potential suppliers to the company, and more.
* **Domain**: A domain is a group of objects, such as users or devices, that share the same AD database.
* **Tree**: A tree is one or more domains grouped together.
* **Forest**: A forest is a group of multiple trees.
* **Organizational Unit (OU)**: Organizational Units (OUs) organize users, groups, and devices. Each domain can contain its own OU.
* **Containers**: Containers and OUs are comparable but container objects cannot be linked or applied to by Group Policy Objects.
* **Trust**: By creating an Active Directory trust (AD trust), two different Active Directory domains (or forests) can be connected so that users in one domain can authenticate against resources in the other.
* **Trusting Domain**: This domain trusts another domain to authenticate users for them.
* **Trusted Domain**: This domain authenticates users on behalf of another domain.
* **Domain controller and AD DS Data Store**
	+ **Domain controller**: Domain controllers are the center of Active Directory. They are in charge of controlling the rest of the domain components.
	
	
		- Functions of Domain controllers
		
		
			+ handles authentication and authorization services
			+ Synchronize updates from additional domain controllers across the entire forest.
			+ Grants administrative access for the management of resources within the domain.
			+ holds the AD DS data store.
	
	
	+ **AD DS Data Store**: All directory information is stored in a data store by the Active Directory directory service. Information on domains, users, groups, machines, organizational units, and security rules are all contained in the directory. The AD DS data store consists of :-
	
	
		- Consists of the Ntds.dit file (Ntds.dit file consist of information about user objects, groups, and group membership. It includes the password hashes for all users in the domain.)
		- Is stored by default in the %SystemRoot%\NTDS folder on all domain controllers
		- Is accessible only through the domain controller processes and protocols
* **Viruses:** Self-replicating programs that spread from one device to another.
* **Botnets:** Networks of compromised devices controlled by a single attacker.
* **Keyloggers:** Software that records keystrokes typed on a keyboard.
* **Ransomware:** Malicious software that encrypts a victim's files and demands a ransom payment for decryption.
* **SQL injection attacks:** Techniques used to inject malicious code into SQL database queries.
* **Man-in-the-middle attacks:** Attacks where a malicious actor intercepts communication between two parties.
* **Phishing attacks and social engineering:** Deceptive tactics used to trick users into revealing sensitive information.
* **Physical surveillance and sabotage:** Physical access to network infrastructure can be exploited for malicious purposes.

**Safeguarding Business Assets: The Importance of Network Security**

Network security is paramount for protecting a business's sensitive data. This includes:

* Employee and customer personal information
* Financial data
* Intellectual property

Data breaches can severely disrupt operations, erode customer trust, and lead to financial losses. Implementing robust network security measures is essential to safeguard these valuable assets.
# Active Directory

![image](https://github.com/fahimalshihab/Network/assets/97816146/d9f59c93-8261-4e5f-a60e-c2df31e745d7)

**What and Why Active Directory**
=============================

**What is Active Directory?**
Active Directory (AD) is a Microsoft technology that helps organizations manage and organize their computer systems, users, and resources. It acts like a digital directory or address book for a network, keeping track of information about users, computers, and other networked devices.

**Why Use Active Directory?**
Some key purposes and benefits of using Active Directory:

* **Centralized Management**: All network resources can be managed and controlled in an organized and centralized manner with the help of Active Directory.
* **User Authentication and Authorization**: It functions as a central authentication system, enabling users to log in with just their username and password and granting access according to their roles and permissions on the network.
* **Security**: Active Directory enables the implementation of security policies and access controls.
* **Group Policy**: Group Policy allows network administrators to apply and enforce settings on several computers at once.
* **Resource Management**: It enables network resources like printers, files, and apps to be arranged and managed in an organized way.
* **Scalability**: The increase in the size of the organization will not affect the functionality of Active Directory.
* **Single sign-on**: Users can utilize a single set of credentials to access a variety of resources and services while using Active Directory.

**Main Terminologies and Components of Active Directory**
=====================================================

* **Objects**: Resources that are present in the AD network are known as objects in Active Directory (AD).
* **Domain**: A domain is a group of objects, such as users or devices, that share the same AD database.
* **Tree**: A tree is one or more domains grouped together.
* **Forest**: A forest is a group of multiple trees.
* **Organizational Unit (OU)**: Organizational Units (OUs) organize users, groups, and devices.
* **Containers**: Containers and OUs are comparable but container objects cannot be linked or applied to by Group Policy Objects.
* **Trust**: By creating an Active Directory trust (AD trust), two different Active Directory domains (or forests) can be connected so that users in one domain can authenticate against resources in the other.
* **Trusting Domain**: This domain trusts another domain to authenticate users for them.
* **Trusted Domain**: This domain authenticates users on behalf of another domain.
* **Domain controller and AD DS Data Store**
  ![image](https://github.com/fahimalshihab/Network/assets/97816146/3197e13e-1e84-45c8-9749-2ce2007cffc5)

	+ **Domain controller**: Domain controllers are the center of Active Directory.
	+ **AD DS Data Store**: All directory information is stored in a data store by the Active Directory directory service.

**Users and Groups**
==================

* **Users**: In Active Directory network, there are four basic categories of users; however, based on an organization’s access management practices, more user types may exist.
	+ **Domain Admins**: These are accounts with administrative privileges at the domain level.
	+ **Service Accounts**: These accounts are used by services and applications to interact with the domain.
	+ **Local Administrator**: This refers to an account that has administrative privileges on a specific computer or device.
	+ **Domain users**: These are standard user accounts that are used by individuals to log in to the domain and access resources for which they have permissions.
* **GROUPS**: Groups make it easier to give permissions to users and objects by organizing them into groups with specified permissions.

**Domain Trusts and Domain Policies**
==================================

* **Domain Trust**: A relationship established between two domains in Active Directory that allows users from one domain to access resources in another domain.
* **Domain Policy**: Typically refers to the security policies and configurations applied to all computers within a specific domain through Group Policy.

**Domain Services**
================

* **Domain Services**: The rest of the domain or tree receives these services from the domain controller. An extensive range of services can be added to a domain controller.
	+ **LDAP**: Lightweight Directory Access Protocol; provides communication between applications and directory services.
	+ **Certificate Services**: Allows the domain controller to create, validate, and revoke public key certificates.
	+ **DNS, LLMNR, NBT-NS**: Domain Name Services for identifying IP hostnames.
