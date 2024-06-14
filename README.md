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

