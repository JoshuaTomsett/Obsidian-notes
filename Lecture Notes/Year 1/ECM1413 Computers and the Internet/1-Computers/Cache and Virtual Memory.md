[[ECM1413 Computers and the Internet]]

20-Oct-2022

### Cache Management

The two methods for deciding what to store in cache are:
- Temporal locality
- Spatial locality


##### Temporal locality

Programs exhibit temporal locality (locality in time). If an item in memory is referenced, then it is likely to be referenced again soon

When a cache needs to discard data, it tends to first discard the data that has not been requested in a long time

##### Spatial locality

Programs exhibit spatial locality (locality in space). If an item in memory is referenced, then it is likely that those nearby will be referenced soon

When a specific memory block is referenced, the cache will often also bring in additional memory blocks located at similar addresses

##### Hits and Misses

A memory request may be:
- a cache hit - read data from cache
- a cache miss - read data from memory into cache first


### Cache Designs

- direct-mapping
- fully-associative mapping
- set-associative mapping

##### Direct-Mapped Cache

In a direct-mapped cache, a memory address is mapped to exactly one cache address

Pros: easy to search

Cons: inefficient use of the cache space


##### Fully-Associative Cache

A memory address is mapped to the least-recently-used cache address

Pros: flexible, can fill the cache with any combination of memory addresses

Cons: takes a long time to search


##### S-Way Set-Associative Cahce

![[Pasted image 20221025174413.png]]


##### Relationship Between Caches

![[Pasted image 20221025174452.png]]


### Reading and Writing

##### Write Hits and Misses

- a write hit - the address we want to write to is present in the cache
- a write miss - the address we want to write to is not present in the cache

##### Dealing with write hits

![[Pasted image 20221025174843.png]]

##### Dealing with write misses

![[Pasted image 20221025174908.png]]

##### Temporal Locality and Writes

![[Pasted image 20221025174953.png]]


### Virtual Memory

Using disk storage as if it was main memory
Main memory is the cache of the disk

Deciding which pages should be loaded:
- Demand paging
- Pre-paging

##### Demand Paging

![[Pasted image 20221025175343.png]]

##### Pre-Paging

![[Pasted image 20221025175359.png]]

##### Page Replacement Algorithms

![[Pasted image 20221025175552.png]]

