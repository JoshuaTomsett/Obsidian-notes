[[ECM1413 Computers and the Internet]]

08-Dec-2022


### Network Gateways

![[Pasted image 20221208123937.png]]


### Firewall Characteristics

A firewall can:
- restrict both incoming and outgoing traffic
- use both positive and negative filters
- consider both the payload and different TCP/IP headers
- consider packets individually or as part of a flow


### Types of Firewalls

The principal types of firewalls are:
- packet-filtering
- stateful packet inspection
- application-level gateways
- curcuit-level gateways


#### Packet Filtering Firewalls

![[Pasted image 20221208124351.png]]

A packet-filtering firewall filters individual packets on the basis of packet headers and packet payloads

![[Pasted image 20221208124437.png]]

##### Wildcard Masks

![[Pasted image 20221208124501.png]]

A wildcard mask indicates which bits of an IP address a particular rule is concerned with during IP address matching

![[Pasted image 20221208124601.png]]


#### Stateful Firewalls

![[Pasted image 20221208124633.png]]

A stateful firewall reviews the same packet infomation as a packet filtering firewall, but also filters packets on the basis of a directory of established transport-layer connections

![[Pasted image 20221208124741.png]]


#### Application-Level Gateway

![[Pasted image 20221208124818.png]]

An application-level gateway filters packets based on applications or certain features of applications

An application-level gateway sets up two TCP connections: one from the trussted network to the firewall, and one from the firewall to the untrusted network

These firewalls can be used as a web or e-mail gateway


#### Circuit-Level Gateway

![[Pasted image 20221208125037.png]]

A circuit-level gateway determines which TCP connections will be allowed. Just as the application-level gateway, a circuit-level gateway sets up two TCP connections

![[Pasted image 20221208125140.png]]


### Firewall Organizations

Firewall organizations include:
- single firewall inline
- double firewall inline


#### Single Firewall Inline

![[Pasted image 20221208125248.png]]


#### Double Firewall Inline

![[Pasted image 20221208125306.png]]


### Virtual Private Networks (VPN)

![[Pasted image 20221208125332.png]]

A VPN uses encryption and authentication to provide a secure connection through an otherwise insecure network, typically the internet


#### VPN Benefits

A VPN can be used to bypass firewalls and other restrictions, and to increase privacy and security


#### VPN Limitations

Using a VPN may result in lower connection speeds, blocks from certain internet services, and resale of your data to third parties

