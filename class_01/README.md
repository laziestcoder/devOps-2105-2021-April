# class 01 : Introduction to DevOps

## Topics:
* Linux, Core Linux, Linux CLI
* RCA (Root Cause Analysis)
* IAC (Infrastructure As Code)
* Cloud Governence
* Linux Namespace
	* User Namespace 
	* Kernal Namespace
* OSI Model (Open Systems Interconnection): APS (Application Layer) | TNDP
	* Application/Software Layer:
		* A : Application Layer
		* P : Presentation Layer
		* S : Session Layer
	* T : Transport Layer -> Heart of OSI Model
	* Hardware Layer: 
		* N : Network Layer
		* D : Data Link Layer
		* P : Physical Layer
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

### telnet:
	* telnet <ip> <port>

### nslookup:
	* nslookup <domain>

### dig:
	* dig <domain>

### for edit hosts file (Domain Parking):
	* `sudo vi/etc/hosts`





