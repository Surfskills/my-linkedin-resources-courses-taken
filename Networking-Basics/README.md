    NETWORK
Network is the collection of interconnected devices.
A network can categorized in two ways: Connectability & Coverage.
    
1. Connectability
- There is a wired connection using an Ethernet cable, which has an eight conductor connector on each end known as an rj45 connector or CAT 5 or CAT 6 cables.
- There is a wireless connection where one can connect to that network, using device's wireless capabilities.
    
2. Coverage
- A Personal Area Network or a PAN, is a very small network that interconnects two devices.
- A Local Area Network or a LAN, is usually local to a building, or maybe just an area within that building.
- A Campus Area Network or a CAN, interconnects nearby buildings.
- Metropolitan Area Network or a MAN evadable, which allows a business to connect all of their offices to a MAN.
- Wide Area Network or a WAN, that interconnects networks over large geographical regions. Maybe we have our corporate offices scattered around the country, maybe around the globe.

N/B: VPNs or Virtual Private Networks allows us to virtually have a private network, which is a more secure network, even though our data is flowing over the public internet.
    
    BENEFITS OF NETWORK
1. Network gives us the ability to share resources.

2. Enhences communication.

3. Network provides redundancy.

5. Provides security through monitoring

6. Network enables internet access.

It enables a single point of administration for network administrators.
   
    NETWORK ADDRESSES
  - Media Access Control address (MAC address) is the specific physical address assigned by manufacturers to networking devices using Network Interface Card(NIC). MAC addresses have 48 bits. The bits are divides into two parts; the first 24 bits are known as the Vendors's code or Organationally Unique Identifier(OUI).
 

  - IP version 4 addresse is a logical address because it's an address that needs to be assigned to the device as opposed to a MAC address, which is coded into the hardware by the manufacturer. 
 

  - An IPv4 address is 32 bits in length, with four different groupings of eight bits separated by dots, and each of these eight bit groupings called octet.
 The first 16 bits of IP4 address represent the network, and the last 16 bits represent the host.
 
 N/B; There are so many network devices in the world, it's not possible for each of them to have a unique IPv4 address, Network Address Translation (NAT) provides a walk around on it.

 IP Version 6 (To be updated with a simpler explanation)
 
 

    PARTS OF A NETWORK.  
- Network Interface Card (NIC) is a circuitry that allow us to send and receive data on either a wired or wireless network.

- A switch is a connective tissue that ties our network devices together. 
- Switches learn what Mac addresses live off of which ports. When a frame comes into the switch destined for a specific Mac address, if the switch already learned the Mac address it will only forward that frame out of the port connecting out to that destination Mac address.


- A router is a device used to interconnect networks. 

When a router is configured with a network it is connected to, that router adds those directly connected networks to its IP routing table. 
In networks with more than one router, those routers can exchange routing information using a routing protocol such as OSPF.


- Copper twisted pair cabling is eight conductors (eight pins) inserted into a connector using a climper tool. Twisting is done to prevent  electromagnetic interference during transmission. 
- There are two types of shielding done to also prevent interference; unshielded twisted pair (UTP) and shielded twisted pair (STP)

 Plenum-rated cable is used in industries and data centers because it does not produce toxic fumes.

 Fiber-optic cabling is used for longer distance connections with an absolutely zero electromagnetic interference.

 There are two primary types of fiber-optic cables; single mode fiber - SMF, and multi-mode fiber - MMF.
 

 Single Mode Fiber is the most preferred because thereis no distortion.

    THE OSI MODEL (Open Systems Interconnection)

Learning the seven layers
![image](https://user-images.githubusercontent.com/99356176/212560091-37f1abce-d894-4fc9-86c8-0481c99cc9fb.png)

OSI helps the network admin categorize hardware and software components and better visualize how they work together.
- The physical layer is where we have things like network cabling or radio waves being sent from wireless access points. At this layer, data is in form of bits.
- Data Link layer is where physical addressing happens using MAC Addresses with ethernet switches. The data is is inform of frames.
- Transport layer is concerned with logical connections. Transmission control protocol (TCP) and user datagram protocol (UDP) operate here. Data is in form of segments.
- Session layer is concerned with establishing, monitoring, and then tearing down communication sessions between our hosts. Here, applications communicate with each other via APIs.
- The presentation layer is concerned with how we represent data. Encryption protocols live here.
- Application layer is the user interface. The HTTP/HTTPS/DNS protocols live here. This protocols enable the user to surf the internet.

N/B: The acrostic, Please Do Not Throw Sausage Pizza Away can help in remembering the layers chronologically , and  Bacon Frying Produces Salivation for data forms in the first four layers.**

    TCP/IP model
- This model combines layers five through seven of the OSI model into a single layer  known as the application layer.
- ![image](https://user-images.githubusercontent.com/99356176/212560193-b16c5dad-54c6-4341-b190-05b036443eba.png)

- It combines the OSI model's physical and data link layers into a single network access layer, and the network layer, it gets renamed as the internet layer.
- It combines combining layers five through seven into that single application layer.
- TCP gives us reliable communication while UDP gives us unreliable communication.

Protocols
![protocols](https://user-images.githubusercontent.com/99356176/212560311-55792005-e8b3-4edb-b38e-b8bf7ec0b9e2.PNG)

 HTTP - Hypertext Transfer Protocol is the protocol used when communicating with traditional web servers. It uses TCP port 80.

 HTTP or Hypertext Transfer Protocol Secure is a secure connection with a web server, protects data from eavesdroppers. It uses TCP port 443

 Both HTTP/HTTPs uses a series of verbs, like POST or GET to send and retrieve information to and from a web server.

    DNS (Domain Name System)
 DNS stands for Domain Name System and communicates with the server that uses either TCP or UDP port 53.
 Routers forward traffic based on IP address information, not names.
 


    DHCP (Dynamic Host Configuration Protocol)
Dynamic Host Configuration Protocol. This is a super useful protocol which gives us a way to automatically assign IP addresses to our network devices without having to visit each device and do a manual configuration and uses UDP port 67.

The communication process ( D-O-R-A )


PC A wants an IP version 4 address, but PC A doesn't know the IP address of the DHCP server that's going to give it that information. 

PC A sends a Discover broadcast asking if there is a DHCP server somewhere out there on the network.
DHCP server receives that discover broadcast, it responds to PC A with an Offer message telling PC A the IP address of the DHCP server.

PC A,send out a Request message asking the DHCP server for IPv4 address information.

DHCP server acknowledges the request message with an  Acknowledgement message, it provides PC A with its IP address, subnet mask, default gateway, maybe other parameters such as the address of a DNS server.

N/B: Where routers are envolved, the router is configured to forward discover broadcasts to the DHCP server.

DHCP Servers for IPV6 Version to be updated on state ansd stateless DHCP v6 servers.

    NAT(Network Address Translation)
NAT allows us to have one set of IP addresses inside of our network and have those IP addresses translated into one or more IP addresses that can be routed on the public internet.

In IPv4, there are some specific ranges of IP addresses that are designated for private use and cannot use them on the public internet.  IP addresses on the inside of our networks have to be translated into one or more publicly ratable IP addresses.

Publicly ratable addresses range between 192.0.2.101 and 192.0.2.199.

Routers are configured for NAT and they take the client ones private IP address of 10.1.1.1, and get it translated to the publicly ratable IP address from that pool.

inside a local address refers to the IP address of a device inside our network while inside globally address refers to the to device on the outside of our network.

Dynamic NAT is dynamically translating multiple inside local addresses into multiple inside global addresses.

    NTP (Network Time Provider)

NTP uses internet-based time sources,. It uses UDP Port 123
Importance. 
 Provides accurate time for the use of digital certificates, which expire at certain dates and times.
 Provides time a certain issue occurred for better and accurate troubleshooting.


    Quality of Service (QoS)
QoS is managed unfairness across the network - traffic in the network is treated differently.

Features of QoS

Classification and marking - classify traffic, early on in its travel, and then market with a priority marking then it lets the next router or the next switch, look at that marking and make a forwarding decision or dropping decision based on that marking.

Queuing -  When a router or switch is receiving traffic faster than it can forward it out, the router or the switch, it allocates some memory called a buffer or a queue to store that traffic.

    Types of wireless LANs
ad hoc wireless network -  Here two wireless devices, they can communicate directly between themselves. It is suitable for ocassional file transfer. Bluethooth.

Infrastructure wireless LAN - Here wireless clients, like laptops or smartphones, they communicate directly with wireless access points hardwired into the network.!
It gives us additional management and monitoring features that we wouldn't have with an ad hoc wireless network; bandwidth utilization and security configuration.


Mesh wireless LAN - These types of access points don't need to be connected to our wired infrastructure. Mesh access point requires power to receive a signal from one access point and then retransmit that wireless signal.

    2.4 GHz vs. 5 GHz wireless networking.

 Wireless LANs use radio frequencies and one of two different bands; 2.4 gigahertz band and the five gigahertz band.

 The 2.4 gigahertz band of frequencies gets divided into channels and we have five megahertz of bandwidth between each of those channels.
Design to avoid overlapping

 The 5 GHz is the popular frequency band for wifi networks. (To be updated)

    Network Design 
 Design is important in preventing wireless access points from interfering with one another. 
 To keep one access point from interfering with another, there is a need to have five channels of separation.
                            (To be updated)


    Antanna

Antanna is used in transmitting and receiving radio waves.

Omnidirectional antenna - They transmit radio waves in all directions perpendicular to the antenna.

MU-MIMO, which stands for multiple user, multiple input, multiple output is a technology used to communicate with multiple clients. 

Directional antenna - They are used to focus radio waves to a specific direction. Coomon in Wi-Fi network.

    Emerging Trends in Networking.
    Software-defined networking (SDN)
SDN enables us to use an application that expresses our intent for network behavior. Then that application can communicate with an SDN controller. That controller then sends appropriate commands out to our network devices all at once.

SDN controller can then be in charge of communicating with all of our devices through Southbound interfaces ( SBI).


An API is something that lets two pieces of software communicate with each other.
Northbound Interfaces (NBI) seats above the SDN controlller.


The specific way the application communicates with the SDN controller is called Representational State Transfer (REST). REST communicates with an SDN controller in much the same way that a web browser communicates with a web server, using HTTP instructions. REST uses these HTTP verbs to send and request information to and from an SDN controller

Extensible Markup Language(XML), and JSON or JavaScript Object Notation is used to format data flowing between an application and an SDN controller. Python language is used to write application programs on NIBs & SBIs.

    Virtualization

 Virtulization is a scenarion where we have a single physical server and install multiple virtual servers on that physical server. 


We can have single physical server hosting on which we install three virtual servers as virtual machines; Microsoft Windows Server, a Linux Server, and an Oracle Solaris Server.

The physical server is running a piece of software called a hypervisor. A hypervisor is software that can create, start, stop and monitor multiple virtual machines.

The virtual machines are logically separate from one another. Each running their own operating system but share resources of the underlying physical computer.

There are two types of hypervisors.



 A type one hypervisor installed on the physical computer without any underlying operating system. Example, VMware's ESXi hypervisor.

 A type two hypervisor that is installed on top of an existing operating system.Example,  VMware's Fusion hypervisor.

Into variants of virtual servers is something called a containers. containers run different applications and have no knowledge of one another sharing the same underlying installation of Microsoft Windows. This reduces the storage space required on that physical server and making each container smaller and more portable.

 Virtulization can be used to virtualize network components like virtual routers and virtual switches.

 We can have these physical servers reside in a data center of a cloud provider. Examples include Amazon Web Services or AWS and Microsoft Azure.

    Cloud Computing

Cloud providers offer us plenty of cloud-based services beyond just providing a remote place to store our data. For example, software as a service or SaaS lets us access applications through a web browser. 


A SaaS application I use a lot is Google's G Suite, which gives me access to Gmail, Google Calendar, Google Sheets, lots of other applications. 

Infrastructure as a service, Software developers often benefit from using platform as a service, or PaaS, to have virtual access to a wide variety of computing platforms that they're developing software for.

Public cloud is when the compute resources are owned and maintained by a cloud provider who shares their compute resources with multiple customers

Private cloud is when company want a dedicated set of compute resources just for our organization's use. A private cloud might be hosted in our own local data center, although it could be hosted by a private cloud service provider.


Many organizations use both public and private cloud computing and that type of deployment is called a hybrid cloud.

N/B; Companies set up a virtual connection between our location and the cloud provider through a virtual private network (VPN) which encrypts data flowing over that VPN.




    5G and Wi-Fi 6
These technologies often run faster than our high speed wired LANs, which might be running at a gigabit per second.  5G is a cellular data service and Wi-Fi 6 is a wireless LAN standard.

    5G (fifth generation of cellular technology).  
It uses an entirely different band of radio frequencies that are much higher frequencies than frequencies used by 3G and 4G. (20 gigabits per second.)


5G use very high frequency in the range from 30 through 300 gigahertz meaning that wavelengths of one of these radio waves is very small on the order of millimeters.These higher frequencies allow us to squeeze more data into a transmission. 
 
 The challenge with that is those high frequencies getting absorbed by walls and windows and lots of other material much more so than frequencies used by 4G.

    Wi-Fi 6(sixth generation of Wi-Fi standards).
                (To be updated)



