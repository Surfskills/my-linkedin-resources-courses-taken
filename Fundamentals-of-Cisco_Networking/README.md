    MULTIPLE ACCESS PROTOCOLS IN COMPUTER NETWORK
The Data Link Layer is responsible for transmission of data between two nodes. Its main functions are- 

    1. Data Link Control
    2. Multiple Access Control

Data Link control – 
    The data link control is responsible for reliable transmission of message over transmission channel by using techniques like framing, error control and flow control.

Multiple Access Control – 
    If there is a dedicated link between the sender and the receiver then data link control layer is sufficient, however if there is no dedicated link present then multiple stations can access the channel simultaneously. Hence multiple access protocols are required to decrease collision and avoid crosstalk
    Multiple access protocols can be subdivided further as – 

    1. Random Access Protocol

    2. Controlled Access

    3. Channelization

Controlled Access

In controlled access, the stations seek information from one another to find which station has the right to send. It allows only one node to send at a time, to avoid collision of messages on shared medium. The three controlled-access methods are:

    1. Reservation
    2. Polling
    3. Token Passing

Channelization

In this, the available bandwidth of the link is shared in time, frequency and code to multiple stations to access channel simultaneously. 

    1. Frequency Division Multiple Access (FDMA)
    2. Time Division Multiple Access (TDMA)
    3. Code Division Multiple Access (CDMA)

Random Access Protocol

In this, all stations have same superiority that is no station has more priority than another station. The Random access protocols are further subdivided as 
    1. ALOHA(Pure and Slotted ALOHA), 
    2. CSMA, 
    3. CSMA/CD & 
    4. CSMA/CA


    Carrier Sense Multiple Access (CSMA)

This method was developed to decrease the chances of collisions when two or more stations start sending their signals over the data link layer. Carrier Sense multiple access requires that each station first check the state of the medium before sending.


    1. Carrier Sense Multiple Access with Collision Detection (CSMA/CD):

In this method, a station monitors the medium after it sends a frame to see if the transmission was successful. If successful, the transmission is finished, if not, in wired networks, if a collision has occurred then the energy of the received signal almost doubles, and the station can sense the possibility of collision.the frame is sent again. 

    2. Carrier Sense Multiple Access with Collision Avoidance (CSMA/CA) –

The basic idea behind CSMA/CA is that the station should be able to receive while transmitting to detect a collision from different stations.  In the case of wireless networks, most of the energy is used for transmission, and the energy of the received signal increases by only 5-10% if a collision occurs. It can’t be used by the station to sense collision. Therefore CSMA/CA has been specially designed for wireless networks. 


 

    NETWORK DEVICES

(Hub, Repeater, Bridge, Switch, Router, Gateways and Brouter)

    1. Repeater 
A repeater operates at the physical layer. Its job is to regenerate the signal over the same network before the signal becomes too weak or corrupted to extend the length to which the signal can be transmitted over the same network. 

    2. Hub   
A hub is a basically multi-port repeater. A hub connects multiple wires coming from different branches. Hubs cannot filter data, so data packets are sent to all connected devices. The hub is neither a collision domain separator nor a broadcast domain separator. All the devices connected to a hub are in a single collision and single broadcast domain.
    
    - Active Hub
These are the hubs that have their power supply and can clean, boost, and relay the signal along with the network. It serves both as a repeater as well as a wiring center. These are used to extend the maximum distance between nodes.

    - Passive Hub 
These are the hubs that collect wiring from nodes and power supply from the active hub. These hubs relay signals onto the network without cleaning and boosting them and can’t be used to extend the distance between nodes.

    - Intelligent Hub 
It works like an active hub and includes remote management capabilities. They also provide flexible data rates to network devices. It also enables an administrator to monitor the traffic passing through the hub and to configure each port in the hub.


    3. Bridge 
A bridge operates at the data link layer. A bridge is a repeater, with add on the functionality of filtering content by reading the MAC addresses of the source and destination. It is also used for interconnecting two LANs working on the same protocol.

    - Transparent Bridges 
These are the bridge in which the stations are completely unaware of the bridge’s existence i.e. whether or not a bridge is added or deleted from the network, reconfiguration of the stations is unnecessary. These bridges make use of two processes i.e. bridge forwarding and bridge learning.

    - Source Routing Bridges
In these bridges, routing operation is performed by the source station and the frame specifies which route to follow. The host can discover the frame by sending a special frame called the discovery frame, which spreads through the entire network using all possible paths to the destination.

    4. Switch 
A switch is a multiport bridge with a buffer and a design that can boost its efficiency(a large number of ports imply less traffic) and performance. A switch is a data link layer device. The switch can perform error checking before forwarding data, which makes it very efficient as it does not forward packets that have errors and forward good packets selectively to the correct port only. The switch is a collision domain separator but not a broadcast separator.

    5. Routers 
A router is a device like a switch that routes data packets based on their IP addresses. The router is mainly a Network Layer device. Routers normally connect LANs and WANs and have a dynamically updating routing table based on which they make decisions on routing the data packets. The router divides the broadcast domains of hosts connected through it.The router is a collision domain separator and a broadcast separator.

    6. Gateway 
A gateway is a passage to connect two networks that may work upon different networking models. They work as messenger agents that take data from one system, interpret it, and transfer it to another system. Gateways are also called protocol converters and can operate at any network layer.

    7. Brouter 
It is also known as the bridging router is a device that combines features of both bridge and router. It can work either at the data link layer or a network layer. Working as a router, it is capable of routing packets across networks and working as the bridge, it is capable of filtering local area network traffic.

    8. NIC 
NIC or network interface card is a network adapter that is used to connect the computer to the network. It is installed in the computer to establish a LAN.  It has a unique id that is written on the chip, and it has a connector to connect the cable to it. The cable acts as an interface between the computer and the router or modem. NIC card is a layer 2 device which means that it works on both the physical and data link layers of the network model. 

    Reference
Data Communications and Networking with TCPIP Protocol Suite, 6/e Paperback – 3 August 2022 by Behrouz A. Forouzan 

    TRANSMISSION MODES IN COMPUTER NETWORKS


Transmission mode means transferring data between two devices. It is also known as a communication mode. Buses and networks are designed to allow communication to occur between individual devices that are interconnected. There are three types of transmission mode:- 

    1. Simplex Mode –
In Simplex mode, the communication is unidirectional, as on a one-way street. Only one of the two devices on a link can transmit, the other can only receive. The simplex mode can use the entire capacity of the channel to send data in one direction. E.g, Keyboard and the monitor

    2. Half-Duplex Mode –
In half-duplex mode, each station can both transmit and receive, but not at the same time. When one device is sending, the other can only receive, and vice versa. The half-duplex mode is used in cases where there is no need for communication in both directions at the same time. E.g Messaging

    3. Full-Duplex Mode –
In full-duplex mode, both stations can transmit and receive simultaneously. In full_duplex mode, signals going in one direction share the capacity of the link with signals going in another direction. E.g Telephone comminication

    COLLISION DOMAIN AND BROADCAST DOMAIN IN COMPUTER NETWORK
.
    Collision Domain – 

A Collision Domain is a scenario in which when a device sends out a message to the network, all other devices which are included in its collision domain have to pay attention to it, no matter if it was destined for them or not. This causes a problem because, in a situation where two devices send out their messages simultaneously, a collision will occur leading them to wait and re-transmit their respective messages, one at a time.

    Broadcast Domain – 

A Broadcast Domain is a scenario in which when a device sends out a broadcast message, all the devices present in its broadcast domain have to pay attention to it. This creates a lot of congestion in the network, commonly called LAN congestion, which affects the bandwidth of the users present in that network. 
From this, we can realize that the more the number of collision domains and the more the number of broadcast domains, the more efficient is the network providing better bandwidth to all its users.


    CISCO WIRELESS ARCHITECTURE AND AP MODES

Cisco Wireless Architecture and AP modes connect a wireless network to a wired network to safely transfer data. Cisco Wireless Architecture and AP modes are classified into three categories: 

    1. Autonomous AP architecture
    2. Cloud-based AP architecture
    3. Split MAC AP architecture.
.
    Autonomous AP architecture

 It provides Central Access Point, which controls all wireless networks and devices through its wireless and wired capabilities. The access point serves as a bridge between the wired and wireless networks. A device linked to an AP wireless network can send data to another wirelessly connected device without using the wired network

    Cloud-Based AP Architecture

 It is necessary in the case of cloud-based AP architecture in order to configure and administer any autonomous AP in the network. The management platform needs to be set up in the internet cloud so that any autonomous AP can be managed and configured from a single location. 

 For centralized management, monitoring the wireless performance, and controlling the actions of wireless autonomous APs, Cisco Wireless Architecture & AP modes employ Cisco Meraki, a cloud-based management solution. Cisco Meraki AP only needs to register with it once; no manual setup or purchases are necessary. All APs will automatically configure themselves in accordance with Cisco Meraki management after registering with the company.

    Split MAC Architecture

 All the network’s autonomous access points (APs) are protected by split MAC structures. Each AP operates under its own security policy. In order to manage security-related concerns, such as intrusion detection and prevention systems, QoS, bandwidth management, a centralized location is used.

 The Autonomous AP management functions include RF power output management, QoS, security management, client authentication, and other management programs. On the other hand, real-time functions are concerned with the transfer of data frames, data encryption and decryption

 Automated AP receives and transfers 802.11 frames in real-time. The autonomous AP communicates with the clients via the physical layer known as the MAC layer.

 The hardware of an autonomous AP is known as a lightweight access point because it solely performs real-time operations. WLC is often in charge of managing autonomous AP (wireless LAN controller)

 Control and Provisioning of Wireless Access Point (CAPWAP) tunneling protocol is used to encapsulate data within a wireless network. The CAPWAP connection is made up of two distinct tunnels, 

    1. CAPWAP control messages for exchanging the codes required to set up and operate the AP.

    2. CAPWAP data for transporting packets between wireless clients linked to a single AP


    INTRODUCTION OF FIREWALL IN COMPUTER NETWORK
 A firewall is a network security device, either hardware or software-based, which monitors all incoming and outgoing traffic and based on a defined set of security rules it accepts, rejects or drops that specific traffic.

    Generation of Firewall or Firewall methodologies

    1. Packet Filtering Firewall.  
    
    Packet filtering firewall is used to control network access by monitoring outgoing and incoming packet and allowing them to pass or stop based on source and destination IP address, protocols and ports. It analyses traffic at the transport protocol layer.

    2. Stateful Inspection Firewall. 
    
    It keeps track of the state of networks connection travelling across it, such as TCP streams. So the filtering decisions would not only be based on defined rules, but also on packet’s history in the state table.

    3. Application Layer Firewall. 
    
    Application layer firewall can inspect and filter the packets on any OSI layer, up to the application layer. It has the ability to block specific content, also recognize when certain application and protocols (like HTTP, FTP) are being misused.

  Application layer firewalls are hosts that run proxy servers. A proxy firewall prevents the direct connection between either side of the firewall, each packet has to pass through the proxy. It can allow or block the traffic based on predefined rules.
  Note: Application layer firewalls can also be used as Network Address Translator(NAT).

    4. Next Generation Firewalls (NGFW) : Next Generation Firewalls are being deployed these days to stop modern security breaches like advance malware attacks and application-layer attacks. NGFW consists of Deep Packet Inspection, Application Inspection, SSL/SSH inspection and many functionalities to protect the network from these modern threats. Example is Cisco ASA with firePOWER.

   Types of Firewall

Firewalls are generally of two types: Host-based and Network-based.

  Host- based Firewalls : Host-based firewall is installed on each network node which controls each incoming and outgoing packet. It is a software application or suite of applications, comes as a part of the operating system. Host-based firewalls are needed because network firewalls cannot provide protection inside a trusted network. Host firewall protects each host from attacks and unauthorized access.

   Network-based Firewalls : Network firewall function on network level. In other words, these firewalls filter all incoming and outgoing traffic across the network. It protects the internal network by filtering the traffic using rules defined on the firewall. A Network firewall might have two or more network interface cards (NICs). A network-based firewall is usually a dedicated system with proprietary software installed.

    References
https://en.wikipedia.org/wiki/Firewall_(computing)
https://www.cisco.com/c/en_in/products/security/firewalls/what-is-a-firewall.html


    INTRUSION PREVENTION SYSTEM (IPS)

It is a network security application that monitors network or system activities for malicious activity. Major functions of intrusion prevention systems are to identify malicious activity, collect information about this activity, report it and attempt to block or stop it. 

 IPS typically record information related to observed events, notify security administrators of important observed events and produce reports. Many IPS can also respond to a detected threat by attempting to prevent it from succeeding. They use various response techniques, which involve the IPS stopping the attack itself, changing the security environment or changing the attack’s content. 

    Intrusion Prevention System (IPS) is classified into 4 types: 
 
    1. Network-based intrusion prevention system (NIPS): 

It monitors the entire network for suspicious traffic by analyzing protocol activity. It detects Network, transport, and application TCP/IP layer activity

    2. Wireless intrusion prevention system (WIPS): 

It monitors a wireless network for suspicious traffic by analyzing wireless networking protocols. It detects Wireless protocol activity; unauthorized wireless local area networks (WLAN) in use.

    3. Network behavior analysis (NBA): 

It examines network traffic to identify threats that generate unusual traffic flows, such as distributed denial of service attacks, specific forms of malware and policy violations. It detects Network, transport, and application TCP/IP layer activity  that causes anomalous network flows

    4. Host-based intrusion prevention system (HIPS): 

It is an inbuilt software package which operates a single host for doubtful activity by scanning events that occur within that host. It detects Host application and operating system (OS) activity; network, transport, and application TCP/IP layer activity
 

