[[ECM1413 Computers and the Internet]]

21-Nov-2022


In the DNS, a client sends a request for the IP address of a specific web address to a server and recieves the IP address as a response back from the server

### Web Addresses

![[Pasted image 20221122192605.png]]

A web address, also know as a Uniform Resource Loader (URL), consists of three parts:
- a protocol identifier
- a host name
- a subdirectory


### Mapping

![[Pasted image 20221122192726.png]]


### Requirements

The DNS must achieve:
- scalability
- efficiency
- reliability
- maintainability


### Scalability

The DNS achieves scalability by organising a large number of servers in a hierarchical fashion

![[Pasted image 20221122192906.png]]


##### Root Servers

There are thirteen roots servers at the top of the hierarchy

Each server root server (IP address) refers to multiple physical servers in multiple locations, this is known as anycast

##### Top-Level Domain Servers

![[Pasted image 20221122193041.png]]

There are many top-level domain servers for contry-based (.us, .uk, .au, .de) and generic (.com, .net, .org)

Top-level domains are managed by ICANN (Internet Corporation for Assigned Names and Numbers)

##### Authorative Servers

![[Pasted image 20221122193225.png]]

There is an authoritative server for every organisation with a publicaly-accessible web or mail server. Ultimately, all mappings between web addresses and IP addresses derive from DNS records held by authoritative servers

##### Host Names

![[Pasted image 20221122193402.png]]


### Efficiency

The DNS achieves efficiency by local server caching. Clients and routers may also use their own DNS caches


### Reliability

There are thirteen root servers distributed throughout the world

![[Pasted image 20221122193955.png]]


### Maintainability

The IP address associated with a website can change due to changes in the web server, in the network configuration, or in the internet serviec provider

Authorative domain servers can be registered, updated and deregistered automatically. These changes then propogate upwards through the tree


### Betryal by a Trusted Server

A trusted DNS server may not be so trustworthy, it may prmote some policy or business relationship


### DNSSEC

The Domain Name System Security Extensions uses:
- asymmetric encryption
- hash functions


#### Asymmetric Encryption

![[Pasted image 20221122194409.png]]


#### Hash Functions

![[Pasted image 20221122194423.png]]


#### Signing a DNS Response

![[Pasted image 20221122194443.png]]


#### Verifying a DNS Response

![[Pasted image 20221122194503.png]]

