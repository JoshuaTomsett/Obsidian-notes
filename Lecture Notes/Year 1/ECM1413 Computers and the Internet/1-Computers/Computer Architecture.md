[[ECM1413 Computers and the Internet]]

17-Oct-2022

### Central Processing unit

Controls the execution of programs
A CPU will usea specific instruction set architecture, such as ARM or x86

#### Registers

- The CPU stores temporary results in internal registers
- When executing a process, that processes registers are loaded into the CPU
- Some registers are interchangable general-purpose registers
- Some registers are special-purpose registers
![[Pasted image 20221017114220.png]]

##### The Base Pointer and Stack pointer

The base pointer points to the start (base) of the current frame
The stack pointer points to the top of the stack

##### The Link Register and Program Counter

The link register stores the address where to return to when the current function call has finished
The program counter stores the address of  the next instrustions to be executed

##### The Arithmetic Logic Unit and Status register

The ALU performs simple operations between two input registers (operands) and puts the result in an output register

The status register contains status and control bits indicating, for example, the output of the ALU and the mode of the CPU


#### Assembly Languages

![[Pasted image 20221017115311.png]]

#### Branching

- Branch instructions jump to a different instruction
- They do this by changing the program counter
- Branches can be conditional or unconditional


### Bits, Bytes, and words

Bit : 0 or 1
Byte : 8 bits
word : may be 2, 4, or 8 bytes / each register is word sized / on a 64 bit machine a word is 8 bytes


### Referencing Registers

- An assembly level instruction often references one or more registers


### Memory hierarchy
![[Pasted image 20221017121008.png]]


### Main Memory

![[Pasted image 20221017121053.png]]
![[Pasted image 20221017121109.png]]


### Number Systems

==Decimal== : Base 10

==Binary== : Base 2

==Octal== : Base 8

==Hexadecimal== : Base 16

![[Pasted image 20221017121718.png]]


#### Applications

Hexacdecimal numbers are used to represnt colour codes using RGB