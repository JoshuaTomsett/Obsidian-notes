[[ECM1415 Discrete Mathematics for Computer Science]]

30-Nov-2022


### Paths

A path of length n from u to v in G is a sequence of n edges e1, ..., en of G

Circuit - a path that begins and ends at the same vertex

Simple path - a path that does not contain the same edge more than once

Cycle - a circuit that does not repeat vertices


### Connectivity

An undirected graph is called connected if there is a path between every pair of verticies
Connected:
![[Pasted image 20221204112332.png]]

Disconnected:
![[Pasted image 20221204112346.png]]

##### Connected Components

A connected component of a graph G is a connected subgraph of G that is not a proper subgraph of another connected subgraph of G

##### Strongly Connected

A directed graph is strongly connected if there is a path from a to b and a path from b to a whenever a and b are verticies in the graph


### Euler Paths and Circuits

Euler circuit - a simple `circuit` containing every edge of G.

Euler path - a simple `path` containinf every edge of G


##### Euler Circuits

![[Pasted image 20221204113200.png]]

![[Pasted image 20221204113250.png]]

![[Pasted image 20221204113324.png]]


### Hamilton Paths and Circuits

Hamilton path - a simple path that passes through every vertex exactly once

Hamilton circuit - a simple circuit that passes through every vertex exactly once


##### Sufficient Conditions for Hamilton Circuits

![[Pasted image 20221204113622.png]]

note: this is not a necessary condition, but a sufficient one


### Planar Graphs

A graph is called planar if it can be drawn in the plane without any edges crossing

Such a drawing of the graph is called a `planar representation` of the graph


#### Euler's Formula

![[Pasted image 20221204114111.png]]
![[Pasted image 20221204114144.png]]


#### Necessary Conditions for Planar Graphs

![[Pasted image 20221204114228.png]]

![[Pasted image 20221204114327.png]]

##### Kuratowski's Theorem

![[Pasted image 20221204114502.png]]

![[Pasted image 20221204114518.png]]

