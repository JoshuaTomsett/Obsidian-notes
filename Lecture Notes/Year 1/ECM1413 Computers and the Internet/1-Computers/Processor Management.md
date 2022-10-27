[[ECM1413 Computers and the Internet]]

10-Oct-2022

### Scheduling Algorithms

- first come first served
- round robin
- shortest process next
- multilevel queuing

##### First Come First Served

Allocates the processor on the basis of creation time (a queue)

Pros : no switching between processes / every process will eventually get done

Cons : average waiting time is often long


##### Round Robin

All processes are in a queue and get a predefined time length to be executed
The process will either be completed, or be interrupted and placed at the end of the circular queue

Pros : resources are distributed "fairly" / quick process can be completed faster

Cons : long average waiting time for large processes / performance depends on time quantum


##### Shortest Process Next

Shares the processor on the basis of shortest predicted execution time

Pros : gives the minimum average waiting time for a given set of processes

Cons : execition time has to be estimated / longer processes  may have to wait a long time


##### Multilevel Queuing

Different queues for different processes (eg: interactive / normal / batch)
Queues are ranked by priority (eg: interactive queue gets 80% of CPU, normal queue gets 10%)
Each queue can have differnent scheduling algorithms

Pros : complex, can accommodate a range of different performance objectives

Cons : complex, difficult to calibrate


### Scheduling Criteria


##### User-Oriented Criteria

Focus on performance as percieved by an individual user, eg: response time


##### System-Oriented Criteria

Focus on efficient utalization of the processor, eg: throughput (number of processes completed per unit time)


### Multi-Processor Scheduling

Each processor / core has its own cache memory
There is a cache hierarchy (L1, L2, L3)

##### Two Approaches to Multi-Processor Scheduling

![[Pasted image 20221016184343.png]]

#### Improving the Performance of Multi-Processor Scheduling


##### Load Balancing

Balance processes evenly among processors
Used by common ready queues


##### Processor Affinity

Keep a process running on the same processor to keep cache warm
Soft affinity : only move processes if there is a good reason
Used by private queues

