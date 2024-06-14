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

# The DHCP Protocol
IP addresses can be assigned either manually, by entering them physically into a device, or automatically and most commonly by using a DHCP (Dynamic Host Configuration Protocol) server. When a device connects to a network, if it has not already been manually assigned an IP address, it sends out a request (DHCP Discover) to see if any DHCP servers are on the network. The DHCP server then replies back with an IP address the device could use (DHCP Offer). The device then sends a reply confirming it wants the offered IP Address (DHCP Request), and then lastly, the DHCP server sends a reply acknowledging this has been completed, and the device can start using the IP Address (DHCP ACK).

![image](https://github.com/fahimalshihab/Network/assets/97816146/61c67e9b-ac94-4aa3-af50-97f36646d74b)



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
