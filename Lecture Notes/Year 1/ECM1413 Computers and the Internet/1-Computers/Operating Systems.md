[[ECM1413 Computers and the Internet]]

26-Sep-2022

Definition : A program that controls the execution of application programs and acts as an interface between applications and the computer hardware
![[Pasted image 20221013193935.png]]

### Services

![[Pasted image 20221013194004.png]]

### The kernel

The most centeral part of an operating system

User mode : certain areas of memory are protected from the user and certain instructions may not be exectued

Kernel mode : all areas of memory are avialable and privillaged instructions may be executed

##### Context switches 
- transition between user mode and kernel mode
- computationally expensive
- an OS should aim to minimise the number of context switches

### Operating System Structures

- Monolithic
- Layered
- Microkernel
- Modular

##### Monolithic

![[Pasted image 20221013194544.png]]
![[Pasted image 20221013194558.png]]

##### Layered

![[Pasted image 20221013194635.png]]
![[Pasted image 20221013194654.png]]
![[Pasted image 20221013194704.png]]

##### Microkernel

![[Pasted image 20221013194739.png]]
![[Pasted image 20221013194751.png]]

##### Modular

![[Pasted image 20221013194815.png]]
![[Pasted image 20221013194825.png]]

##### Virtual Machines

- a host operating system provides virtual hardware to one or multiple guest operating systems
- enables multiple enviroments on one machine