# Netwhat
My repositories for the 21 (42) schools "Netwhat" project 

## Netwhat test's <a name="test"></a>

> Link: [click](https://github.com/adblanc/netwhat42-train)  
> 
> Run Test  `./netwhat42 37`

**1. ◦ What is an IP address**

> IP address stands for internet protocol address. It is an identifying
> number that is associated with a specific computer or computer
> network. When connected to the internet, the IP address allows the
> computers to send and receive information.
>
> IP Addres is composed of: **[ network ] [ host ]** IP Addres Example:
> **66.171.248.170**

 **2. ◦ What is a Netmask**

> Netmask is a term used in computer networking to define the class and
> range of Internet Protocol (IP) addresses. Netmask provides the
> available number range of IP addresses From Class A to Class C, and
> specifies a mask to divide these networks into sub-networks (subnets).
>
> Netmask primarily provides a method to create small subnetworks from a
> large range of IP addresses. Generally, netmask length is defined in
> up to 24-bit format for all types of IP classes. The division or
> creation of networks into subnetworks depends on the class of IP
> address in use along with their available netmasks. For example, the
> netmasks for the three IP classes are:
>
> - **255.0.0.0** for **Class A** with an **8-bit** netmask
> - **255.255.0.0** for **Class B** with a **16-bit** netmask
> - **255.255.255.0** for **Class C** with a **24-bit** netmask
>
> The greater the length of netmask the more networks it can://avinetworks.com/glossary/subnet-mask/ Broadcasts
> increases.

 **3. What is the subnet of an IP with Netmask**
>  A subnet mask is a 32-bit number created by setting host bits to all
> 0s and setting network bits to all 1s. In this way, the subnet mask
> separates the IP address into the network and host addresses.
>
> The “255” address is always assigned to a broadcast address, and the
> “0” address is always assigned to a network address. Neither can be
> assigned to hosts, as they are reserved for these special purposes.
>
> The IP address, subnet mask and gateway or router comprise an
> underlying structure—the Internet Protocol—that most networks use to
> facilitate inter-device communication.
>
> When organizations need additional subnetworking, subnetting divides
> the host element of the IP address further into a subnet. The goal of
> subnet masks are simply to enable the subnetting process. The phrase
> “mask” is applied because the subnet mask essentially uses its own
> 32-bit number to mask the IP address.

 **4. What is the broadcast address of a subnet**

> Highest IP address in a subnet or network, used as the destination IP
> address for broadcast messages.
>  A **broadcast address** is an **IP address** that is used to target
> all systems on a specific **subnet** network instead of single hosts.
> In other words **broadcast address** allows information to be sent to
> all machines on a given **subnet** rather than to a specific machine.

**5. What are the different ways to represent an IP address with the Netmask**


> Netmask is a 32-bit "mask" used to divide an IP address into subnets
> and specify the network's available hosts.
>
> 255.255.255.0 is applied to the 129.144.41.101 , the result is the IPv4 address of 129.144.41.0
>
> 129.144.41.101  **AND**  255.255.255.0 =  **129.144.41.0**
>
> In binary form, the operation is:
>
> **10000001.10010000.00101001.01100101**		<== (IPv4 address)
> AND
> **11111111.11111111.11111111.00000000**		<==(netmask)

 **6. What are the differences between public and private IPs**


> Private IP Address and Public IP Address are used to uniquely identify
> a machine on the internet. Private IP address is used with a local
> network and public IP address is used outside the network. Public IP
> address is provided by ISP, Internet Service Provider.
>
> Following are the important differences between Private IP Address and Public IP Address.

Key|Private IP| Public IP|
|--|--|--|
|**Scope**|Private IP address scope is local to present network.|Public IP Address is used to communicate outside the network.|
**Communication**|Private IP Address is used to communicate within the network.|Public IP Address is used to communicate outside the network.|
**Format**|Private IP Addresses differ in a uniform manner.|Public IP Addresses differ in varying range.|
**Provider**|Local Network Operator creates private IP addresses using network operating system.|ISP, Internet Service Provider controls the public IP address.|
**Cost**|Private IP Addresses are free of cost.|Public IP Address comes with a cost.|
**Locate**|Private IP Address can be located using ipconfig command.|Public IP Address needs to be searched on search engine like google.|
**Range**|Private IP Address range: 10.0.0.0  –  10.255.255.255, 172.16.0.0  –  172.31.255.255,192.168.0.0  –  192.168.255.255| Public IP Address needs to be searched on search engine like google.|Except private IP Addresses, rest IP addresses are public.
**Example**|Private IP Address is like 192.168.11.50.| Public IP Address is like 17.5.7.8.
|  |  |  |

 **7. What is a class of IP addresses**
> With an IPv4 IP address, there are five classes of available IP
> ranges: Class A, Class B, Class C, Class D and Class E, while only A,
> B, and C are commonly used. Each class allows for a range of valid IP
> addresses, shown in the following table.
>
Class|Address Range| Supports|
|--|--|--|
**Class A**|1.0.0.1 **to** 126.255.255.254|Supports **16 million** hosts on each of **127 networks**.|
**Class B**|128.1.0.1 **to** 191.255.255.254|Supports **65,000** hosts on each of **16,000 networks**.|
**Class C**|192.0.1.1 **to** 223.255.254.254|Supports **254** hosts on each of **2 million networks**.|
**Class D**|224.0.0.0 **to** 239.255.255.255|Reserved for **multicast** groups.|
**Class E**|240.0.0.0 **to** 254.255.255.254|Reserved for future use, or research and development purposes.|

 **8. What is TCP**

>  The **Transmission Control Protocol** (**TCP**) is one of the main
> protocols of the Internet protocol suite. It originated in the initial
> network implementation in which it complemented the Internet Protocol
> (IP). Therefore, the entire suite is commonly referred to as _TCP/IP_.
> **TCP provides reliable, ordered, and error-checked delivery of a stream of octets (bytes) between applications running on hosts
> communicating via an IP network.**
>
> -   Keeps track of lost packages, makes sure that lost packages are re-sent
> -   Addes sequesce numbers to packets and reorders any packets that arrive in thenworng order.
> -   Slower, because of all added additional functionality.
> -   Requieres more computer resources, because the OS needs to keep track of ongoing communication sessions and manage them on a much
> deeper level.


 **9. What is UDP**

> The User Datagram Protocol, or UDP, is a communication protocol used
> across the Internet for especially time-sensitive transmissions such
> as video playback or DNS lookups. It speeds up communications by not
> formally establishing a connection before data is transferred. This
> allows data to be transferred very quickly, but it can also cause
> packets to become lost in transit
> Like all  networking protocols, UDP is a standardized method for
> transferring data between two computers in a network. Compared to
> other protocols, UDP accomplishes this process in a simple fashion: it
> sends packets (units of data transmission) directly to a target
> computer, without establishing a connection first, indicating the
> order of said packets, or checking whether they arrived as intended.
> (UDP packets are referred to as ‘datagrams’.)
> UDP is faster but less reliable than  TCP, another common transport
> protocol. In a TCP communication, the two computers begin by
> establishing a connection via an automated process called a
> ‘handshake.’ Only once this handshake has been completed will one
> computer actually transfer data packets to the other.
>
> UDP communications do not go through this process. Instead, one
> computer can simply begin sending data to the other.
> -   Doesn't keep track of lost packages
> -   Doesn't care about package arrival order.
> -   Faster, bacause it lacks any extra features.
> -   Requieres less computer resources.
> -   Examples of programs and services that use UPD:
>     -   DNS
>     -   IP telephony
>     -   DHCP
>     -   Many computer games
>     **Why we use UDP?**
>
> Many applications that requiere real-time communication prefer to use
> UDP, applications that requiere speed and that torerat partial data
> loss.

**10. What are the network layers**
> In the seven-layer OSI model of computer network, the network layer is
> layer 3. The network layer is responsible for packet forwarding
> including routing through intermediate routers.
> Anything that has to do with inter-network connections takes place at the network layer. This includes setting up the routes for data packets to take, checking to see if a server in another network is up and running, and addressing and receiving IP packets from other networks. This last process is perhaps the most important, as the vast majority of Internet traffic is sent over IP.

 **11. What is the OSI model**


> The Open Systems Interconnection (OSI) Model is a description of how
> the Internet works. It breaks down the functions involved in sending
> data over the Internet into seven layers. Each layer has some function
> that prepares the data to be sent over wires, cables, and radio waves
> as a series of bits.
>
> The seven layers of the OSI model are:
>
> 1.  **Application layer:** Data generated by and usable by software applications. The main protocol used at this layer is HTTP.
> 2.  **Presentation layer:** Data is translated into a form the application can accept. Some authorities consider HTTPS encryption and decryption to take place at this layer.
> 3.  **Session layer:**  Controls connections between computers (this can also be handled at layer 4 by the  TCP protocol.
> 4.  **Transport layer:**  Provides the means for transmitting data between the two connected parties, as well as controlling the quality of service. The main protocols used here are TCP and UDP.
> 5.  **Network layer:**  Handles the routing and sending of data between different networks. The most important protocols at this layer are IP and ICMP.
> 6.  **Data link layer:**  Handles communications between devices on the same network. If layer 3 is like the address on a piece of mail, then layer 2 is like indicating the office number or apartment number at that address. Ethernet is the protocol most used here.
> 7.  **Physical layer:**  Packets are converted into electrical, radio, or optical pulses and transmitted as bits (the smallest possible units of information) over wires, radio waves, or cables.
>
> It is important to keep in mind that the OSI model is an abstract
> conceptualization of the processes that make the Internet work, and
> interpreting and applying the model to the real-world Internet is
> sometimes a subjective exercise.
>
> The OSI model is useful for helping people talk about networking
> equipment and protocols, determining which protocols are used by which
> software and hardware, and showing roughly how the Internet works. But
> it is not a rigid step-by-step definition of how Internet connections
> always function.

 **12. What is a DHCP server and the DHCP protocol**



> A **DHCP Server** is a network server that automatically
>     provides and assigns IP addresses, default gateways and other
>     network parameters to client devices. It relies on the standard
>     protocol known as Dynamic Host Configuration Protocol or DHCP
>     to respond to broadcast queries by clients.
>
>
>   Dynamic Host Configuration Protocol **(DHCP)** is a client/server
> protocol that automatically provides an Internet Protocol (IP) host
> with its IP address and other related configuration information such
> as the subnet mask and default gateway.

 **13. What is a DNS server and the DNS protocol**


> The Domain Name System
> DNS is the phonebook of the Internet. When users type domain names such as
> ‘google.com’ or ‘nytimes.com’ into web browsers, DNS is responsible
> for finding the correct IP
> address for those sites. Browsers then use those addresses to communicate with origin
> servers or CDN edge servers to access website information. This all happens thanks to DNS servers:
> machines dedicated to answering DNS queries.

The Domain Network System (DNS) protocol helps Internet users and network devices discover websites using human-readable hostnames, instead of numeric IP addresses.

> **The DNS process, simplified, works as follows:**
>
> 1.  A browser, application or device called the  **DNS client**, issues a  **DNS request or DNS address lookup**, providing a hostname such as “example.com”.
> 2.  The request is received by a  **DNS resolver**, which is responsible for finding the correct IP address for that hostname. The DNS resolver looks for a  **DNS name server** that holds the IP address for the hostname in the DNS request.
> 3.  The resolver starts from the Internet’s  **root DNS server**, moving down the hierarchy to Top Level Domain (TLD) DNS servers (“.com” in this case), down to the name server responsible for the
> specific domain “example.com”.
> 4.  When the resolver reaches the  **authoritative DNS name server** for “example.com”, it receives the IP address and other relevant details, and returns it to the DNS client. The DNS request is now **resolved**.
> 5.  The DNS client device can connect to the server directly using the correct IP address.

 **14. What are the rules to make 2 devices communicate using IP addresses**


 **15. How does routing work with IP**



>  Routing is the process by which data packets move from one node
> (machine or device) to another on a computer network until the packets
> reach the final destination.
> The header information includes:
> -   The IP addresses of the source and destination nodes.
> -   Packet numbers that help reassemble the packets in the correct order whe the packets reach the destination.
> -   Other useful technical information.

 **16. What is a default gateway for routing**


> It allows devices within one network to send information to devises within another network. If you are requestiong a certain web page, the trafic is first sent to your default gateay before leaving the local network to reach its indended destination.

**17. What is a port from an IP point of view and what is it used for when connecting to another device**

> In computer networking, a port is a communication endpoint. At the software level, within an operating system, a port is a logical construct that identifies a specific process or a type of network service. Ports are identified for each protocol and address combination by 16-bit unsigned numbers, commonly known as the port number. The most common protocols that use port numbers are the Transmission Control Protocol (TCP) and the User Datagram Protocol (UDP).
