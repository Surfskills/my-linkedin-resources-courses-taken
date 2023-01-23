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
A repeater operates at the physical layer. Its job is to regenerate the signal over the same network before the signal becomes too weak or corrupted to extend the length to which the signal can be transmitted over the same network

    2. Hub   
A hub is a basically multi-port repeater. A hub connects multiple wires coming from different branches. Hubs cannot filter data, so data packets are sent to all connected devices. 
    
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
A switch is a multiport bridge with a buffer and a design that can boost its efficiency(a large number of ports imply less traffic) and performance. A switch is a data link layer device. The switch can perform error checking before forwarding data, which makes it very efficient as it does not forward packets that have errors and forward good packets selectively to the correct port only

    5. Routers 
A router is a device like a switch that routes data packets based on their IP addresses. The router is mainly a Network Layer device. Routers normally connect LANs and WANs and have a dynamically updating routing table based on which they make decisions on routing the data packets. The router divides the broadcast domains of hosts connected through it.

    6. Gateway 
A gateway is a passage to connect two networks that may work upon different networking models. They work as messenger agents that take data from one system, interpret it, and transfer it to another system. Gateways are also called protocol converters and can operate at any network layer.

    7. Brouter 
It is also known as the bridging router is a device that combines features of both bridge and router. It can work either at the data link layer or a network layer. Working as a router, it is capable of routing packets across networks and working as the bridge, it is capable of filtering local area network traffic.

    8. NIC 
NIC or network interface card is a network adapter that is used to connect the computer to the network. It is installed in the computer to establish a LAN.  It has a unique id that is written on the chip, and it has a connector to connect the cable to it. The cable acts as an interface between the computer and the router or modem. NIC card is a layer 2 device which means that it works on both the physical and data link layers of the network model. 

    Reference
Data Communications and Networking with TCPIP Protocol Suite, 6/e Paperback – 3 August 2022 by Behrouz A. Forouzan 

    Transmission Modes in Computer Networks 


Transmission mode means transferring data between two devices. It is also known as a communication mode. Buses and networks are designed to allow communication to occur between individual devices that are interconnected. There are three types of transmission mode:- 

    1. Simplex Mode –
In Simplex mode, the communication is unidirectional, as on a one-way street. Only one of the two devices on a link can transmit, the other can only receive. The simplex mode can use the entire capacity of the channel to send data in one direction. E.g, Keyboard and the monitor

    2. Half-Duplex Mode –
In half-duplex mode, each station can both transmit and receive, but not at the same time. When one device is sending, the other can only receive, and vice versa. The half-duplex mode is used in cases where there is no need for communication in both directions at the same time. E.g Messaging

    3. Full-Duplex Mode –
In full-duplex mode, both stations can transmit and receive simultaneously. In full_duplex mode, signals going in one direction share the capacity of the link with signals going in another direction. E.g Telephone comminication








