[[ECM1413 Computers and the Internet]]

05-Dec-2022


### Multiple Access Protocols

There are two sorts of multiple access protocol:
- Carrier sense, multiple access / collision detection (CSMA/CD) for wired connections
- Carrier sense, multiple access / collision avoidance (CSMA/CA) for wireless connections


### CSMA/CD

![[Pasted image 20221205181201.png]]

- All computers  are attached to a shared cable - Multiple Acces (MA)
- Any computer may transmit of the cable is unused - Carrier Sense (CS)

##### Collision detection

- While transmitting, a computer may detect that it is recieving a message
- After deteting a collision, a computer waits for a random interval, and then tries again

##### Random Waiting Time

- By using a random interval we avoid repeated collisions
- The random intervals are chosen from an exponetially-doubling range


### CSMA/CA

![[Pasted image 20221205184355.png]]

- All computers use a shared frequency - Multiple Access (MA)
- any computer may transmit if the frequency is clear - Carrier Sense (CS)

##### Collision Avoidance

- A computer finding the frequency clear, transmits after an instant
- A computer finding the frequency busy counts down from a random value while the channel is clear; otherwise, the count is frozen - Collision Avoidace (CA)
- A computer then transmits and hopfully recieves an acknowledgement

##### The Hidden Node Problem

A computer may be in range of the base station, but out of range of another computer

![[Pasted image 20221205185222.png]]

The hidden node problem may be solved by reservation using ready to send and clear to send messages


### Collsion-Free Protocols

- Token Ring
- Bit-Map Protocols
- Binary Countdown

##### Token Ring

![[Pasted image 20221205185526.png]]

In a token ring network, a token continuously circulates, to which messages may be attached, and from which they may be removed


##### Bit-Map Protocols

![[Pasted image 20221205185649.png]]

In a bit-map protocol, host n may announce that it has a frame to dend by inserting a 1 bit into slot n

Following this, host begins to transmit frames in numerical order


##### Binary Countdown

![[Pasted image 20221205190006.png]]

Hosts that wish to transmit broadcast their binary address. Hosts with 1's in their address get priority. The winner of the bid gets to transmit a frame