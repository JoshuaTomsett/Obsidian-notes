[[ECM1413 Computers and the Internet]]

28-Nov-2022


![[Pasted image 20221130155341.png]]


### Services

- addressing
- forwarding
- routing
- reporting


### Addressing

The IP gives every host and router network interface an address

##### Headers

![[Pasted image 20221130155702.png]]

The most important fields of an IP packet header are the source address and destination address


##### Dotted Decimal Notation

![[Pasted image 20221130155806.png]]

IP addresses are written in dotted decimal notation: bytes are written as decimal numbers. seperated by dots

![[Pasted image 20221130155858.png]]


##### Network Prefix and Host Suffix

![[Pasted image 20221130160006.png]]


##### Slash (CIDR) Notation

![[Pasted image 20221130160031.png]]


##### Subnet Masks and CIDR Notation

![[Pasted image 20221130160053.png]]


##### Subnetting

![[Pasted image 20221130160112.png]]
![[Pasted image 20221130160123.png]]

##### Public and Private Addresses

Certain private addresses may not be used on the public internet


### Forwarding

![[Pasted image 20221130160218.png]]

A router forwards packets on the appropiate interface according to their addresses

##### Forwarding Tables

![[Pasted image 20221130160313.png]]

A router stores a forwarding table which specifies an interface for each possible destination address

##### Longest Prefix Address Matching

![[Pasted image 20221130160450.png]]

Forwarding tables use longest prefix address matching


### Routing

A router periodically exchanges routing metrics with its neighbours, and then recomputes its forwarding table

##### Hierarchial IP Addressing

![[Pasted image 20221130161126.png]]


### Reporting

The Internet Control Messaging Protocol (ICMP) allows hosts and routers to communicate infomation to each other

##### ICMP Messages

![[Pasted image 20221130162418.png]]


### IPv4 Address Space Exhaustion

In October 2015, the poll of address (2^32) are exhausted.

#### Conserving IP Addresses

- Network address translation
- Classless inter-domain routing

##### Network Address Translation (NAT)

![[Pasted image 20221201121904.png]]

##### Classless Inter-Domain Routing (CIDR)

![[Pasted image 20221201121935.png]]
Avoids giving some hosts to many addresses