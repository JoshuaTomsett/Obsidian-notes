[[ECM1413 Computers and the Internet]]

13-Oct-2022

### Processes

A process is a program in execution
Mulitple processes may be active at once
Each process is represented by a process control block which is stored in memory


### Memory Management Tasks

- relocation
- protection
- sharing

#### Relocation

A memory management technique needs to be able to relocate a process to a new place in memory

#### Protection

All processes need to be protected against interference from other processes

#### Sharing

Process may sometimes need to share data


### Memory Management Techniques


#### Fixed partitioning

- Memory is divided into partitions of a fixed size; the size may vary between partitions
- A process can be loaded into any partition whose size is equal to or greater than the size of the process
- One-to-one mapping between partitions and processes
- Internal fragmentation : space is wasted inside partitions when the size of a process is smaller than the size of the partition

Pros : easy to understand and implement

Cons : internal fragmentation / pre-specified upper limit on the size of processes


#### Dynamic Partitioning

- The partition sizes adjust to the sizes of processes
- One-to-one mapping between processes and partitions
- External fragmentation : space is wasted between partitions
- Compaction : shift processes so that they are contiguous and so that all free memory is gathered in one continuous block

![[Pasted image 20221016191408.png]]

Pros : no internal fragmentation / no limit on size of processes

Cons : external fragmentation / time is wasted on compaction


#### Simple Segmentation

- Each program is divided into segments
- Segments are loaded into memory as in dynamic partitioning
- All segments need to be loaded into memory, but they do not need to be contiguous

![[Pasted image 20221016191647.png]]

Pros : easier to fit processes in memory

Cons : exernal fragmentation (less than dynamic partitioning)


#### Virtual Memory Segmentation

- Use disk storage as if it was main memory
- Segments are loaded into memory as in dynamic partitioning, except that not all segments need to be loaded at the same time

![[Pasted image 20221016191906.png]]

Pros : easier to fit processes in memory than with simple segmentation

Cons : more overhead required for virtual memory


#### Simple Paging

- Memory is divided into fixed-size frames of equal size
- Each process is divided into pages of the same size
- Internal fragmentation is small sinceit only affects the last frame of each process

Pros : all pages fit perfectly into frames

Cons : each process requires a page table (which consumes memory)


#### Virtual Memory Paging

Pages are loaded into frames as in simple paging, except that not all pages need to be loaded at the same time

![[Pasted image 20221016192337.png]]

Pros : easier to fit processes in memory than simple paging

Cons : more overhead required


#### Protection and Sharing with Segmentation and Paging

![[Pasted image 20221016192457.png]]

