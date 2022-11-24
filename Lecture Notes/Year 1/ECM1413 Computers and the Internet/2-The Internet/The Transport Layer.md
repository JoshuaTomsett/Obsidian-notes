[[ECM1413 Computers and the Internet]]

24-Nov-2022


### The Protocols

- Transmission Control Protocol - TCP
- User Datagram Protocol - UDP


### Header and Payload

![[Pasted image 20221124121331.png]]


### Application Layer and TCP

![[Pasted image 20221124121356.png]]


### The TCP Header

![[Pasted image 20221124121415.png]]


### Networking Ports

![[Pasted image 20221124121437.png]]


### The TCP Services

- connection-oriented communication
- end-to-end communication
- complete reliability
- full duplex communication
- a stream interface
- reliable connection startup
- graceful connection shutdown


#### Conncetion-Oriented Communication

- The TCP provides connection oriented communication - an application sets up a connection, uses it, and tears it down

#### End-to-End Communication

- A connection has exactly two endpoints

#### Complete Reliability

- Data will be recieved exactly as sent, even if that means resending

#### Full-Duplex Communication

- Data may be sent and recieved simultaneously

#### A Stream Interface

- A continuous stream of data is sent and recieved

#### Reliable Connection Startup

![[Pasted image 20221124130834.png]]

#### Graceful Connection Shutdown

![[Pasted image 20221124130946.png]]


### UDP Header

![[Pasted image 20221124131005.png]]


### UDP Services

- Connectionless communication
- End-to-end communication
- Best-effort reliability
- A message interface


#### Connectionless Communication

- An application does not set up or tear down a connection

#### End-to-End Communication

- A connection has exactly two endpoints

#### Best-Effort Reliability

- Data may be lost, duplicated, or delayed

#### A Message Interface

- Individual data items are sent and recieved (no data stream)


### TCP vs UDP

TCP provides full reliability, with high latency

UDP provides best-effort reliability, with minimal latency

Examples:
- DNS would use UDP
- FTP would use TCP
- video game player movement would use UDP
- video streaming would use TCP