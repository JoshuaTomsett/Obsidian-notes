[[ECM1415 Discrete Mathematics for Computer Science]]

23-Nov-2022


### Graphs

A graph G = (V, E) consists of a nonempty set V of vertices and a set E of edges

- Each edge has one or two verticies associated with it, called its endpoints
- An edge is said to connect its endpoints

##### Terminology

Simple graph:
- each edge connects two different verticies and no two edges connect the same pair of verticies.
![[Pasted image 20221124111444.png]]

Multigraphs:
- may have multiple edges connecting the same two verticies. When m different edges connect u and v, we say that { u , v} is an edge of multiplicity m.
![[Pasted image 20221124111509.png]]

Pseudograph:
- may include loops, as well as multiple edges connecting the same pair of verticies
![[Pasted image 20221124111606.png]]


### Direct Graphs

A directed graph (or digraph) G = (V, E) consists of a nonempty set V of verticies and a set E of directed edges

- each edge is associated with an ordered pair of verticies ( u , v)
- such an edge is said to start at u and end at v
- u is the initial vertex of the edge and is adjacent to v and v is the terminal vertex of the edge and is adjacent to from u
- the initial and terminal verticies of a loop are the same
![[Pasted image 20221124112003.png]]

##### Terminology

Simple directed graph:
- has no loops and no multiple edges

Directed multigraph:
- may have multiple direct edges. When there are m direct edges from the vertex u to the vertex v, we say that ( u , v) is an edge of multiplicity m


![[Pasted image 20221124112219.png]]


### Basic Terminology

The set of all neighbors of a vertex v of G = (V, E), denoted by N(v), is called the neighborhood of v. If A is a subset of V, we denote by N(A) the set of all vertices in G that are adjacent to at least one vertex in A.

![[Pasted image 20221124112600.png]]

The degree of a vertex in an undirected graph is the number of edges incident with it, except that a loop at a vertex contributes two to the degree of that vertex. The degree of the vertex v is denoted by $deg(V)$.


#### Degrees and Neighborhoods

![[Pasted image 20221124112814.png]]

![[Pasted image 20221124112912.png]]
![[Pasted image 20221124113447.png]]
![[Pasted image 20221124113508.png]]
![[Pasted image 20221124113558.png]]


### Simple Types of Simple Graphs

##### Complete graphs

![[Pasted image 20221124113654.png]]

##### Cycles

![[Pasted image 20221124113711.png]]

##### Wheels

![[Pasted image 20221124113729.png]]

##### n-Cubes

![[Pasted image 20221124113746.png]]


### Bipartite Graphs

A simple graph G is bipartite if V can be partitioned into disjoint subsets V1 and V2 such that every edge connects a vertex in V1 and a vertex in V2. In other words, there are no edges which connect two vertices in V1 or in V2

![[Pasted image 20221124114007.png]]

##### Complete Bipartite Graphs

![[Pasted image 20221124114036.png]]


### Matchings

A matching M in a simple graph G = (V, E) is a subset of the set E of edges of the graph such that no two edges are incident with the same vertex. In other words, a matching is a subset of the edges such that if {s,t} and {u,v} are distinct edges of the matching, then s, t, u, v are distinct.

![[Pasted image 20221124115449.png]]

##### Complete matching from V1 to V2

![[Pasted image 20221124115518.png]]

##### Hall's Marriage Theorem

![[Pasted image 20221124115607.png]]


### New Graphs from Old

A subgraph of a graph G = (V, E) is a graph (W, F), where W $\subset$ V and F $\subset$ E. A subgraph H of G is a proper subgraph of G if H $\neq$ G

![[Pasted image 20221124120015.png]]
![[Pasted image 20221124120029.png]]
![[Pasted image 20221124120050.png]]


### Graph Isomorphism

![[Pasted image 20221124121139.png]]
![[Pasted image 20221124121150.png]]
