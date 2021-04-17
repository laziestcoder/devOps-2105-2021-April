# class 01 : Introduction to DevOps


* **DevOps** : *DevOps is borned to handle scaling and monitoring traffic. DevOps is not for either Development portion or Operations. DevOps is mostly connect to developments and operations. Developments knowledge is more important here. DevOps should know most of the technical knowledges of development phase.* 

## Topics:
* CI/CD
* Docker
* Kubernetes
* AWS (Amazon Web Servic) / MS Azure Cloud / GCP (Google Cloud Platform)
* Linux, Core Linux, Linux CLI
* RCA (Root Cause Analysis)
* IAC (Infrastructure As Code)
* Cloud Governence
* Linux Namespace
	* **User Namespace**: User space is set of locations where normal user processes run. These processes can't access kernel space directly. User space refers to all of the code in an operating system that lives outside of the kernel.
	* **Kernal Namespace**: The kernel provides abstraction for security, hardware, and internal data structures. Role of kernel space is to manage applications/ processes running in user space. Processes running under the kernel has access to all of the memory, whereas the user space have access only to a limited part of memory.
* OSI Model (Open Systems Interconnection): APS (Application Layer) | TNDP
	* Application/Software Layer:
		* **A** : Application Layer
		* **P** : Presentation Layer
		* **S** : Session Layer
	* **T** : Transport Layer -> Heart of OSI Model
	* Hardware Layer: 
		* **N** : Network Layer
		* **D** : Data Link Layer
		* **P** : Physical Layer
* Socket Binding
* Host Namespace 
* Network Namespace
* File Namespace
* ARP (Address Resolution Protocol)
	* ARP Request
	* ARP Routing
* Route Table
* CIDR (Classless Inter Domain Routing)

## Goal:
* Docker
* Kubernetes
* Microservices Architecture Design
* Scalability


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
	* IP4 > [0.0.0.0 = 8 bit 2^32] > IP = Logical Address 
	* MAC = Physical Address (Unique Hexadecimal Number which is burnt to LAN Card)
	* VNIC = Virtual Network Interface Card
	* 
	|Cable -> |NIC -> |Kernal Namespace -> |User Namepace|
	|--|--|--|--|
	|Physical|Interface/Software|eth0|Application|
* Interface :
* MTU (Maximum Transation Unit):
* UDP (User Datagram Protocol):
* TCP (Transmission Control Protocol):
* Payload: Payload and Data are same.
* DNS (Domain Name Sequence):
	* DNS Query:
	* DNS Resolve:
	* DNS Cache:
* TTL (Time To Leave):
* NAT (Network Address Translation): 

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
* ```tcpdump -i en0``` - data-network packet analyzer/monitoring dns queries
querying DNS to obtain domain name or IP address mapping
* ```telnet 52.74.245.254 443``` - connect to a remote host
* ```tcpdump -i en0 | grep -i "UDP"```
* ```tcpdump -i eth0 dst 52.74.245.254 443``` - to see traffic
* ```nc -l 8000``` - NetCat Web server
* ```ipaddr show```





