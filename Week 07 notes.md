# CIT 114 Week 7
## Here are some important things I learned in Week 7
### Notes 05: Networking & Content Delivery

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

Virtual Private Cloud (VPC) - is a public cloud offering that lets a group establish its own private cloud-like computing environment on shared public cloud infrastructure.

#### IP Addressing in your VPC

IP addresses enable resources in your VPC to communicate with each other, and with resources over the Internet. 

By default, Amazon EC2 and Amazon VPC use the IPv4 addressing protocol. When you create a VPC, you must assign it an IPv4 CIDR block (a range of private IPv4 addresses). Private IPv4 addresses are not reachable over the Internet. To connect to your instance over the Internet, or to enable communication between your instances and other AWS services that have public endpoints, you can assign a globally-unique public IPv4 address to your instance.

You can optionally associate an IPv6 CIDR block with your VPC and subnets, and assign IPv6 addresses from that block to the resources in your VPC. IPv6 addresses are public and reachable over the Internet.

To ensure that your instances can communicate with the Internet, you must also attach an Internet gateway to your VPC. For more information, see Internet gateways.

VPC can operate in dual-stack mode: your resources can communicate over IPv4, or IPv6, or both. IPv4 and IPv6 addresses are independent of each other; you must configure routing and security in your VPC separately for IPv4 and IPv6.

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
_____________________________
Private IPv4 addresses (also referred to as private IP addresses in this topic) are not reachable over the Internet, and can be used for communication between the instances in your VPC. When you launch an instance into a VPC, a primary private IP address from the IPv4 address range of the subnet is assigned to the default network interface (eth0) of the instance. Each instance is also given a private (internal) DNS hostname that resolves to the private IP address of the instance. If you don't specify a primary private IP address, we select an available IP address in the subnet range for you.

Public IPv4 address (also referred to as a public IP address) are given to all subnets that have an attribute that determines whether a network interface created in the subnet. Therefore, when you launch an instance into a subnet that has this attribute enabled, a public IP address is assigned to the primary network interface (eth0) that's created for the instance. A public IP address is mapped to the primary private IP address through network address translation (NAT).

You can optionally associate an IPv6 CIDR block with your VPC and subnets. Your instance in a VPC receives an IPv6 address if an IPv6 CIDR block is associated with your VPC and your subnet, and if one of the following is true:
   * Your subnet is configured to automatically assign an IPv6 address to the primary network interface of an instance during launch.
   * You manually assign an IPv6 address to your instance during launch.
   * You assign an IPv6 address to your instance after launch.
   * You assign an IPv6 address to a network interface in the same subnet, and attach the network interface to your instance after launch.

When you create a subnet, it requires its own CIDR block. For each CIDR block that you specify, AWS reserves five IP addresses within that block, and these addresses are not available for use. AWS reserves these IP addresses for:
   * Network address
   * VPC local router (internal communications)
   * Domain Name System (DNS) resolution
   * Future use
   * Network broadcast address

#### Elastic Network Interfaces

An elastic network interface (referred to as a network interface in this documentation) is a virtual network interface that can include the following attributes:
   * a primary private IPv4 address
   * one or more secondary private IPv4 addresses
   * one Elastic IP address per private IPv4 address
   * one public IPv4 address, which can be auto-assigned to the network interface for eth0 when you launch an instance
   * one or more IPv6 addresses
   * one or more security groups
   * a MAC address
   * a source/destination check flag
   * a description

#### VPC Route Tables

A route table contains a set of rules, called routes, that are used to determine where network traffic from your subnet or gateway is directed. Each route specifies a destination and a target. The destination is the destination CIDR block where you want traffic from your subnet to go. The target is the target that the destination traffic is sent through. By default, every route table that you create contains a local route for communication in the VPC. You can customize route tables by adding routes. You cannot delete the local route entry that is used for internal communications.

The following are the key concepts for route tables.
   * Main route table - The route table that automatically comes with your VPC. It controls the routing for all subnets that are not explicitly associated with any other route table.
   * Custom route table - A route table that you create for your VPC.
   * Edge association - A route table that you use to route inbound VPC traffic to an appliance. You associate a route table with the internet gateway or virtual private gateway, and specify the network interface of your appliance as the target for VPC traffic.
   * Route table association - The association between a route table and a subnet, internet gateway, or virtual private gateway.
   * Subnet route table - A route table that's associated with a subnet.
   * Gateway route table - A route table that's associated with an internet gateway or virtual private gateway.
   * Local gateway route table - A route table that's associated with an Outposts local gateway.
   * Destination - The range of IP addresses where you want traffic to go (destination CIDR). For example, an external corporate network with a 172.16.0.0/12 CIDR.
   * Propagation - Route propagation allows a virtual private gateway to automatically propagate routes to the route tables. This means that you don't need to manually enter VPN routes to your route tables. 
   * Target - The gateway, network interface, or connection through which to send the destination traffic; for example, an internet gateway.
   * Local route - A default route for communication within the VPC.

#### Internet Gateway

An internet gateway is a horizontally scaled, redundant, and highly available VPC component that allows communication between your VPC and the internet. An internet gateway serves two purposes: to provide a target in your VPC route tables for internet-routable traffic, and to perform network address translation (NAT) for instances that have been assigned public IPv4 addresses. An internet gateway supports IPv4 and IPv6 traffic. It does not cause availability risks or bandwidth constraints on your network traffic.

To enable access to or from the internet for instances in a subnet in a VPC, you must do the following:
   * Attach an internet gateway to your VPC.
   * Add a route to your subnet's route table that directs internet-bound traffic to the internet gateway. If a subnet is associated with a route table that has a route to an internet gateway, it's known as a public subnet. If a subnet is associated with a route table that does not have a route to an internet gateway, it's known as a private subnet.
   * Ensure that instances in your subnet have a globally unique IP address (public IPv4 address, Elastic IP address, or IPv6 address).
   * Ensure that your network access control lists and security group rules allow the relevant traffic to flow to and from your instance.

#### Virtual Private Networks

VPN stands for Virtual Private Network. This technology allows a user to connect one remote private network to a seperate remote private network through a secure virtual tunnel over the public internet. 

There are multiple ways to create this kind of network connection. You can connect your Amazon VPC to remote networks and users using the following VPN connectivity options.

|VPN connectivity option|Description|
|---|---|
|AWS Site-to-Site VPN|You can create an IPsec VPN connection between your VPC and your remote network. On the AWS side of the Site-to-Site VPN connection, a virtual private gateway or transit gateway provides two VPN endpoints (tunnels) for automatic failover. You configure your customer gateway device on the remote side of the Site-to-Site VPN connection.|
|AWS Client VPN|AWS Client VPN is a managed client-based VPN service that enables you to securely access your AWS resources or your on-premises network. With AWS Client VPN, you configure an endpoint to which your users can connect to establish a secure TLS VPN session. This enables clients to access resources in AWS or an on-premises from any location using an OpenVPN-based VPN client.|
|AWS VPN CloudHub|If you have more than one remote network (for example, multiple branch offices), you can create multiple AWS Site-to-Site VPN connections via your virtual private gateway to enable communication between these networks.|
|Third party software VPN appliance|You can create a VPN connection to your remote network by using an Amazon EC2 instance in your VPC that's running a third party software VPN appliance. AWS does not provide or maintain third party software VPN appliances; however, you can choose from a range of products provided by partners and open source communities.|


