[[ECM1413 Computers and the Internet]]

6-Oct-2022

A program : a set of instructions for performing a specific task

A proccess : a program in execution


### Process Lifecycle

![[Pasted image 20221015163108.png]]

==born== : a process has been created but has not yet been asmitted to the pool of executable processes

==ready== : when the OS is ready, the process is transfered to the ready state

==running== : the process is executed by a processor. The process may transfer between the ready state and running processes based on the priority its been assigned by the processor

==waiting== : the process has made a request that it has to wait for; this could input from an I/O device, or access to a file on disk

==died== : the process has been completed or aborted


### Process Control Blocks

Each process is represented by a process control block (PCB). The process control block is stored in memory (or on disk)

Contains:
- process ID
- process state (its registers)
- process address space (its memory)
- process I/O


### Context switching

Multiple processes are active at the same time

to switch from process A t process B:
- change the process scheduling state of A
- save the context of A
- load the context of B
- change the process scheduling state of B

The time a context switch takes is dependent on several factors, including the number of registers that must be copied


### Process Address Space

The sections are:
- a stack section for temporary data
- a heap section for dynamically-allocated data
- a data section for static data
- a text section for program code
![[Pasted image 20221015164327.png]]

Data and text sections have a fixed size

The stack and heap sections can shrink and grow during run time

##### The Stack

When a function is called, temporary variables are added to the top of the stack

When exiting a function, these variables are removed from the top of the stack

Operations : push / pop

last in - first out principle

##### The Heap

Dynamically allocated like the stack

In the heap blocks of memory are allocated and removed in an arbitrary order

Used when you need to store a large block of memory for a long period of time, or for variables that can change size dynamically


### Process Spawning

A process is created at the request of a different process
![[Pasted image 20221015164838.png]]

The initial process is the parent, the new process is called the child

==fork== : creates a child process with a unique process ID, the child is given a copy of the parents process address space

==exec== : runs an executable file that overwrites the process address space with a new program

==wait== : the parent process is put in the waiting state until the child process has finished

==exit== : when done, the child process issues the exit system call, abd the parent process can resume


### Interprocess Communication

Processes may benefit from sharing data with other processes

This is implemented using either `shared memory` or `message passing`

##### Shared Memory

![[Pasted image 20221015165741.png]]

##### Message Passing

![[Pasted image 20221015165803.png]]

##### Pros of Each

Shared memory is faster

Message passing is better for small amounts of data as it is doesnt have a start up cost

