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

#### Understanding TCP/IP addressing and subnetting basics

IP addresses: Networks and hosts

IP address - is a 32-bit number that uniquely identifies a host (computer or other device, such as a printer or router) on a TCP/IP network.

TCP/IP (Transmission Control Protocol/Internet Protocol) - a suite of communication protocols used to interconnect network devices on the internet. TCP/IP is also used as a communications protocol in a private computer network (an intranet or extranet).

Subnet mask - used by the TCP/IP protocol to determine whether a host is on the local subnet or on a remote network.

Network classes

Internet addresses are allocated by the InterNIC, the organization that administers the Internet. These IP addresses are divided into classes. The most common of these are classes A, B, and C. Classes D and E exist, but are not generally used by end users. Each of the address classes has a different default subnet mask. You can identify the class of an IP address by looking at its first octet. Following are the ranges of Class A, B, and C Internet addresses, each with an example address:

   * Class A networks use a default subnet mask of 255.0.0.0 and have 0-127 as their first octet. The address 10.52.36.11 is a class A address. Its first octet is 10, which is between 1 and 126, inclusive.
   * Class B networks use a default subnet mask of 255.255.0.0 and have 128-191 as their first octet. The address 172.16.52.63 is a class B address. Its first octet is 172, which is between 128 and 191, inclusive.
   * Class C networks use a default subnet mask of 255.255.255.0 and have 192-223 as their first octet. The address 192.168.123.132 is a class C address. Its first octet is 192, which is between 192 and 223, inclusive.

Subnetting - the further dividing of a network (ex: A Class A, B, or C TCP/IP network)

Glossary:
   * Broadcast address -- An IP address with a host portion that is all ones.
   * Host -- A computer or other device on a TCP/IP network.
   * Internet -- The global collection of networks that are connected together and share a common range of IP addresses.
   * InterNIC -- The organization responsible for administration of IP addresses on the Internet.
   * IP -- The network protocol used for sending network packets over a TCP/IP network or the Internet.
   * IP Address -- A unique 32-bit address for a host on a TCP/IP network or internetwork.
   * Network -- There are two uses of the term network in this article. One is a group of computers on a single physical network segment; the other is an IP network address range that is allocated by a system administrator.
   * Network address -- An IP address with a host portion that is all zeros.
   * Octet -- An 8-bit number, 4 of which comprise a 32-bit IP address. They have a range of 00000000-11111111 that correspond to the decimal values 0- 255.
   * Packet -- A unit of data passed over a TCP/IP network or wide area network.
   * RFC (Request for Comment) -- A document used to define standards on the Internet.
   * Router -- A device that passes network traffic between different IP networks.
   * Subnet Mask -- A 32-bit number used to distinguish the network and host portions of an IP address.
   * Subnet or Subnetwork -- A smaller network created by dividing a larger network into equal parts.
   * TCP/IP -- Used broadly, the set of protocols, standards and utilities commonly used on the Internet and large networks.
   * Wide area network (WAN) -- A large network that is a collection of smaller networks separated by routers. The Internet is an example of a very large WAN.

IPv4 and IPv6 characteristics and restrictions 
|IPv4|IPv6|
|---|---|
|The format is 32-bit, 4 groups of up to 3 decimal digits.|The format is 128-bit, 8 groups of 4 hexadecimal digits.|
|Default and required for all VPCs; cannot be removed. |Opt-in only.|
|The VPC CIDR block size can be from /16 to /28.	|The VPC CIDR block size is fixed at /56.|
|The subnet CIDR block size can be from /16 to /28.	|The subnet CIDR block size is fixed at /64.|
|You can choose the private IPv4 CIDR block for your VPC.	|We choose the IPv6 CIDR block for your VPC from Amazon's pool of IPv6 addresses. You cannot select your own range.|
|There is a distinction between private and public IP addresses. To enable communication with the Internet, a public IPv4 address is mapped to the primary private IPv4 address through network address translation (NAT). |No distinction between public and private IP addresses. IPv6 addresses are public.|
|Supported on all instance types.	|Supported on all current generation instance types and the C3, R3, and I2 previous generation instance types. For more information, see Instance types.|
|Supported in EC2-Classic, and EC2-Classic connections with a VPC via ClassicLink. |Not supported in EC2-Classic, and not supported for EC2-Classic connections with a VPC via ClassicLink.|
|Supported on all AMIs. |Automatically supported on AMIs that are configured for DHCPv6. Amazon Linux versions 2016.09.0 and later and Windows Server 2008 R2 and later are configured for DHCPv6. For other AMIs, you must manually configure your instance to recognize any assigned IPv6 addresses.|
|An instance receives an Amazon-provided private DNS hostname that corresponds to its private IPv4 address, and if applicable, a public DNS hostname that corresponds to its public IPv4 or Elastic IP address. |Amazon-provided DNS hostnames are not supported.|
|Elastic IPv4 addresses are supported. |Elastic IPv6 addresses are not supported.|
|Supported for AWS Site-to-Site VPN connections and customer gateways, NAT devices, and VPC endpoints. |Not supported for AWS Site-to-Site VPN connections and customer gateways, NAT devices, and VPC endpoints.|
