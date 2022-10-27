[[ECM1413 Computers and the Internet]]

3-Oct-2022

### I/O devices

enable computers to recieve or ouput infomation to humans or devices

##### Buses

The communication with I/O devices is performed over a bus
The I/o devices are operated using controllers (embedded processors)
![[Pasted image 20221015154052.png]]

##### Controller registers

The processor communicates with the controller by reading and writing to the controller's registers

Data-in register : data coming from device
Data-out register : data going to device
Status register : indicating status of device
Control register : commands to device

##### Port-based I/O

The cpu uses special instructions for transferring a small number of bytes to I/O bus address

##### Memory-mapped I/O

The cpu treats the device as memory, control registers are mapped to specific memory addresses

Today memory-mapped I/O is more common than port-based I/O


### Polling

The cpu repeatedly checks the controller's status register to see wheather the controller is busy

When the controller is ready and the CPU wants to give new instructions the CPU writes to the data-out register and signals that it has done so through the controll register

Polling may be better than interrupts if the CPU has notting better to do


### Interrupts

The CPU regularly sences an interrupt-request line

When the CPU gets an interrupt signal through the interrupt-request line, it stops the current process and initiates a response

Interrupts are much more commonly used


### Large data transfers

Some devices (eg: disk drives) will often do large data transfers

The transfer will be inefficient if the CPU has to feed data byte by byte to the controller's registers

A better approach is to offload this work to a special-purpose processor, a direct memory access controller (DMA)

##### Direct Memory Access

The CPU writes a command block into memory, specifying the source and desitation of the transfer

The DMA controller can then perform multiple transfers via a single command

When the transfer is complete, the CPU recieves an interrupt from the DMA controller

This enables the CPU to spend more resources on other tasks


### Device drivers

Provides an interface between I/O devices and the OS
![[Pasted image 20221015155757.png]]


### System calls of I/O devices

- Character I/O
- Block I/O
- Network I/O

#### Character I/o

eg: keyboards, mice

Transfers bytes one by one in the order that they arive

Get operation : returns the next character in the stream
Put operation : adds characters to the stream
Libaries for line-by-line access (eg: backspace to remove the preceding character from the stream)

#### Block I/O

Used to transfer blocks of data

Has read and write operations

Block devices are high volume devices

##### Memory mapped files

Layered on top of block device drivers

Instead of read and write operations a memory-mapped interface provides access to disk storage via a location in main memory; there is a system call that maps a file on the device to memory

The OS deals with transferring data between memory and the device and can perform transfers when needed

Accessing memory-mapped files is faster than using read/write operatiosn since it does not require a contrext switch

#### Network I/O

System calls for :
- creating and connecting sockets
- sending and recieving over the connection
- select function to determine that status of sockets (whether the socket is ready for reading or writing)

With network I/O devices things routinely go wrong (missing packets)

Therefore, there needs to be system functions for checking wheather a transfer was successful and for recovering gracefullt from unsuccessful transfers
