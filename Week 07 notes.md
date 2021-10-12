# CIT 114 Week 7 (Notes 05: Networking & Content Delivery)
## Here are some important thinkgs I learned in Week 6
### Cloud Security

#### What is a Network?

A computer network is just two or more client machines that are connected together, using a network device, to share resources. A network can be logically partitioned to create subnets. A router or switch are used to connect the clients together and enable communications.

#### Definitions for Computer Networking

Computer Network - is the interconnection of multiple devices, generally termed as Hosts connected using multiple paths for the purpose of sending/receiving data or media.

There are also multiple devices or mediums which helps in the communication between two different devices which are known as Network devices. Ex: Router, Switch, Hub, Bridge.

The layout pattern using which devices are interconnected is called as network topology. Such as Bus, Star, Mesh, Ring, Daisy chain.
_____________________________
OSI - stands for Open Systems Interconnection. It is a reference model that specifies standards for communications protocols and also the functionalities of each layer.

The OSI Model layers are as follows: (Anagram: All People Seem To Need Data Processing)
   * Layer 7 - Application
The application layer is the OSI layer closest to the end user, which means both the OSI application layer and the user interact directly with the software application.
   * Layer 6 - Presentation
The presentation layer establishes context between application-layer entities, in which the application-layer entities may use different syntax and semantics if the presentation service provides a mapping between them.
   * Layer 5 - Session
The session layer controls the dialogues (connections) between computers. It establishes, manages and terminates the connections between the local and remote application.
   * Layer 4 - Transport
The transport layer provides the functional and procedural means of transferring variable-length data sequences from a source to a destination host, while maintaining the quality of service functions.
   * Layer 3 - Network
The network layer provides the functional and procedural means of transferring variable length data sequences (called packets) from one node to another connected in "different networks".
   * Layer 2 - Data Link
The data link layer provides node-to-node data transfer—a link between two directly connected nodes
   * Layer 1 - Physical
Responsible for the transmission and reception of unstructured raw data between a device and a physical transmission medium.

Protocol - the set of rules or algorithms which define the way how two entities can communicate across the network and there exists different protocol defined at each layer of OSI model. Few of such protocols are TCP, IP, UDP, ARP, DHCP, FTP and so on.
_____________________________
Unique Identifiers of Network

Host name - a unique device name used to differniate each device on a network

Type “hostname” in the command prompt and press ‘Enter’, this displays the hostname of your machine.
______________________________
IP Address (Internet Protocol address) - also know as Logical Address, is the network address of the system across the network.

To identify each device in the world-wide-web, Internet Assigned Numbers Authority (IANA) assigns IPv4 (Version 4) address as a unique identifier for each device on the Internet. However there is also an IPv6 (Version 6) scheme available that has more addresses available.

Length of the IPv4 address is 32-bits. (Hence we have 2^32 IP addresses available.)

Type “ipconfig” in the command prompt and press ‘Enter’, this gives us the IP address of the device.
_____________________________
Classless Inter-Domain Routing (CIDR) - A common method to describe networks

The CIDR address is expressed as follows:
   * An IP address (which is the first address of the network)
   * Next, a slash character (/)
   * Finally, a number that tells you how many bits of the routing prefix must be fixed or allocated for the network identifier

ex: 192.0.2.0/24
The last number (24) tells you that the first 24 bits must be fixed. The last 8 bits are flexible, which means that 28 (or 256) IP addresses are available for the network, which range from 192.0.2.0 to 192.0.2.255. The fourth decimal digit is allowed to change from 0 to 255.

There are two special cases:
   * Fixed IP addresses, in which every bit is fixed, represent a single IP address (for example, 192.0.2.0/32). This type of address is helpful when you want to set up a firewall rule and give access to a specific host.
   * The internet, in which every bit is flexible, is represented as 0.0.0.0/0
_____________________________
MAC Address (Media Access Control address) - the unique identifier of each host and is associated with the NIC (Network Interface Card). Also known as physical address

MAC address is assigned to the NIC at the time of manufacturing.

Length of the MAC address is : 12-digit/ 6 bytes/ 48 bits

Type “ipconfig/all” in the command prompt and press ‘Enter’, this gives us the MAC address.
_____________________________
Port - can be referred to as a logical channel through which data can be sent/received to an application. Any host may have multiple applications running, and each of this application is identified using the port number on which they are running on.

Port number is a 16-bit integer, hence we have 216 ports available which are categorized as shown below:
   * Well known Ports 0–1023
   * Registered Ports 1024–49151
   * Ephemeral Ports 49152–65535

Number of ports: 65,536

Range: 0–65535

Type “netstat -a” in the command prompt and press ‘Enter’, this lists all the ports being used.
_____________________________
Socket - the unique combination of IP address and Port number together
_____________________________
DNS (Domain Name System) Server - a server which translates web addresses or URL into their corresponding IP addresses. We don’t have to remember all the IP addresses of each and every website.

The command ‘nslookup’ gives you the IP address of the domain you are looking for. This also provides the information of our DNS Server.

ARP (Address Resolution Protocol) - is used to convert the IP address to its corresponding Physical Address(i.e.MAC Address).

ARP is used by the Data Link Layer to identify the MAC address of the Receiver’s machine.

RARP (Reverse Address Resolution Protocol) - provides the IP address of the device given a physical address as input. But RARP has
become obsolete since the time DHCP has come into the picture.
