# class 01 : Introduction to DevOps


**DevOps** : *DevOps is borned to handle scaling and monitoring traffic. DevOps is not for either Development portion or Operations. DevOps is mostly connect to developments and operations. Developments knowledge is more important here. DevOps should know most of the technical knowledges of development phase.* 


## Topics:
* CI/CD
* Docker
* Kubernetes
* AWS (Amazon Web Servic) / MS Azure Cloud / GCP (Google Cloud Platform)
* Linux, Core Linux, Linux CLI
* **RCA** (Root Cause Analysis): *A root cause is defined as a factor that caused a nonconformance and should be permanently eliminated through process improvement. The root cause is the core issue—the highest-level cause—that sets in motion the entire cause-and-effect reaction that ultimately leads to the problem(s).*
* **IaC** (Infrastructure As Code): *Infrastructure as Code is the process of managing and provisioning computer data centers through machine-readable definition files, rather than physical hardware configuration or interactive configuration tools.*
* **Cloud Governence**: *Cloud Governance is a carefully designed set of rules and protocols put in place by businesses that operate in a cloud environment to enhance data security, manage risks, and keep things running smoothly.*
* **Linux Namespace**:
	* **User Namespace**: *User space is set of locations where normal user processes run. These processes can't access kernel space directly. User space refers to all of the code in an operating system that lives outside of the kernel.*
	* **Kernal Namespace**: *The kernel provides abstraction for security, hardware, and internal data structures. Role of kernel space is to manage applications/ processes running in user space. Processes running under the kernel has access to all of the memory, whereas the user space have access only to a limited part of memory.*
  
   ***N.B: Processes running in user space also don't have access to the kernel space. User space processes can only access a small part of the kernel via an interface exposed by the kernel - the system calls. When a system call is executed the arguments to the call are passed from user space to kernel.***

* OSI Model (Open Systems Interconnection): APS (Application Layer) | TNDP
	* Application/Software Layer:
		* **A** : Application Layer
		* **P** : Presentation Layer
		* **S** : Session Layer
	* **T** : *Transport Layer* -> Heart of OSI Model
	* Hardware Layer: 
		* **N** : *Network Layer*
		* **D** : *Data Link Layer*
		* **P** : *Physical Layer*
* **Socket Binding** : *Socket binding is basically assigning an address to it by which, it will be listening for requests to connect to that particular address.*
* **Polling**: *Polling is the continuous checking by a controlling device or process of other devices, processes, queues, etc. in some defined sequence to see what state they are in and whether they need attention (such as whether they are still connected, want to communicate, contain tasks to be executed).*
* **Web server**: *A web server is software and hardware that uses HTTP and other protocols to respond to client requests. The basic objective of the web server is to store, process and deliver web pages to the users.*
* **Host Namespace**: *It is main namespace also know as **Namespace** Namespaces are a feature of the Linux kernel that partitions kernel resources such that one set of processes sees one set of resources while another set of processes sees a different set of resources. The feature works by having the same namespace for a set of resources and processes, but those namespaces refer to distinct resources. Resources may exist in multiple spaces. Examples of such resources are process IDs, hostnames, user IDs, file names, and some names associated with network access, and interprocess communication.*.
* **Network Namespace**: *A network namespace is a logical copy of the network stack from the host system. Each namespace has its own IP addresses, network interfaces, routing tables, and so forth. The default or global namespace is the one in which the host system physical interfaces exist.*
* **File Namespace**: *A namespace is a group of related elements that each have a unique name or identifier. ... Each element within a namespace has a "local name" that serves as a unique identifier. Namespaces are used in many areas of computing, such as domain names, file paths, and XML documents*
* ARP (Address Resolution Protocol)
	* ARP Request
	* ARP Routing
	* ARP Cache
	* ARP Cache Timeout
	* ARP Response/Reply
   
   ***Reverse ARP is being used when host computer/machine don't know their own IP address.***

* **Route Table**: *A routing table, or routing information base (RIB), is a data table stored in a router or a network host that lists the routes to particular network destinations, and in some cases, metrics (distances) associated with those routes.* Below there is an example of Routing Table:

|Network destination | Netmask| Gateway | Interface |
|---|---|---|---
|0.0.0.0|0.0.0.0|192.168.0.1|192.168.0.100|
|127.0.0.0|	255.0.0.0|127.0.0.1|127.0.0.1|
|192.168.0.0| 255.255.255.0|	192.168.0.100| 192.168.0.100|
|192.168.0.100|	255.255.255.255|	127.0.0.1|	127.0.0.1|
|192.168.0.1|	255.255.255.255|	192.168.0.100|	192.168.0.100|

* **CIDR (Classless Inter Domain Routing)**: *It is a set of Internet protocol (IP) standards that is used to create unique identifiers for networks and individual devices. The IP addresses allow particular information packets to be sent to specific computers.*

* **Netcat webserver**: *The Netcat utility program supports a wide range of commands to manage networks and monitor the flow of traffic data between systems.*


## Goal:
* Docker
* Kubernetes
* Microservices Architecture Design
* Scalability
* CI/CD
* AWS/GCP/MS AC


## Notes:
* IPV4: 
* IPV6:
* IP (Internet Protocol):
* Address:
	* Logical Address
	* Physical Address
* MAC (Media Access Control):
* NIC (Network Interface Card):
	* eth0 (Ethernet Interface): This is first ethernet interface. Additional Ethernet interfaces would be named eth1, eth2, etc.
	* lo0 (Loopback Interface)
	* IPV4 > [0.0.0.0 = 8 bit 2^32] > IP = Logical Address 
	* MAC = Physical Address (Unique Hexadecimal Number which is burnt to LAN Card)
	* VNIC = Virtual Network Interface Card
	* |Cable -> |NIC -> |Kernal Namespace -> |User Namepace|
          |--|--|--|--|
	  |Physical|Interface/Software|eth0|Application|

* **Interface** : *It's a device or a system that unrelated entities use to interact. According to this definition, a remote control is an interface between you and a television set, the English language is an interface between two people, and the protocol of behavior enforced in the military is the interface between people of different ranks.*
* MTU (Maximum Transation Unit):
* UDP (User Datagram Protocol):
* TCP (Transmission Control Protocol):
* Payload: Payload and Data are same.
* **DNS** (Domain Name Sequence):
	* **DNS Query**: *A DNS query (also known as a DNS request) is a demand for information sent from a user's computer (DNS client) to a DNS server. In most cases a DNS request is sent, to ask for the IP address associated with a domain name. There is some Command line tools for DNS query. Such as, ```dig```, ```nslookup```, ```host```*
	* DNS Resolve:
	* DNS Cache:
* TTL (Time To Leave):
* NAT (Network Address Translation): 
* CLI (Command Line Interface):

## Ports:
	* 53	: DNS
	* 22	: SSH
	* 80	: TCP
	* 8080	: http
	* 443	: https
	* 123	: UDP
## Commands:

* telnet: ```telnet <ip> <port>```
* nslookup: querying DNS to obtain domain name or IP address mapping ```nslookup <domain>```
* dig: querying DNS nameservers for information ```dig <domain>```
* for edit hosts file (Domain Parking): ```sudo vi/etc/hosts```
* ```ifconfig``` - show list of interfaces
* ```tcpdump -i en0``` - data-network packet analyzer/monitoring dns queries. Querying DNS to obtain domain name or IP address mapping
* ```telnet 52.74.245.254 443``` - connect to a remote host
* ```tcpdump -i en0 | grep -i "UDP"```
* ```tcpdump -i eth0 dst 52.74.245.254 443``` - to see traffic
* ```nc -l 8000``` - NetCat Web server, netcat server for viewing web request response of localhost:8000 using CLI
* ```ipaddr show```
* ```arp -an``` - display the ARP table




