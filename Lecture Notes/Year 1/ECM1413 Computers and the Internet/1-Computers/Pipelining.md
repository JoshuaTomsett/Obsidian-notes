[[ECM1413 Computers and the Internet]]

24-Oct-2022

### Fetch-Decode-Execute Cycle

Fetch - read an instruction from memory
Decode - identify the instruction
Execute - carry out the instruction

![[Pasted image 20221107193936.png]]

##### Time

Clock cycle time - time it takes to complete one pipelining stage
Clock speed - 1 / Clock cycle time
Execution time - Clock cycles for program X Clock cycle time


### Control and Data Control Hazards

#### Control Hazards

Occurs when a conditional branch instruction changes the next instruction
There are 4 ways to deal with control hazards:
- Stall the pipeline
- Assume branch not taken
- Branch prediction
- Branch delay slots

##### Stall the pipeline

The processor may stall the pipeline; when we realise that the next instruction is a branch instruction

Pros: dont need to guess the next instruction
Cons: time and resources are wasted


##### Assume branch not taken

The processor may assume branch not taken, squashing instructions if wrong

Pros: dont need to guess the next instruction
Cons: time and resources are wasted when branch not taken


##### Branch prediction

The processor may try branch prediction based on past branches. If the prediction is incorrect, instructions are squashed

Pros: can significantly reduce the number of wasted clock cycles
Cons: overhead associated with the branch prediction


##### Branch delay slots

A branch instruction may be followed by delay slots

Pros: may find useful instructions
Cons: if no useful instruction is found, fill the slot with "no operation"


#### Data Hazards

A data hazard occurs when an instruction requires a result from a previous instruction before that result has been computed/written

Types of data hazards:
- Read after Write (RAW)
- Write after Read (WAR)
- Write after Write (WAW)

