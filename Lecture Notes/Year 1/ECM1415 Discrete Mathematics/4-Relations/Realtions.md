[[ECM1415 Discrete Mathematics for Computer Science]]

19-Oct-2022

### Relations

##### Tuples

![[Pasted image 20221022134145.png]]

![[Pasted image 20221022134200.png]]


##### Binary Relations

![[Pasted image 20221022134311.png]]

![[Pasted image 20221022134323.png]]


##### Digraphs

![[Pasted image 20221022134435.png]]

![[Pasted image 20221022134456.png]]


##### Composition

R1 $\subseteq$ A X B
R2 $\subseteq$ B X C

R2 $\circ$ R1 $\subseteq$ A X C

![[Pasted image 20221022143449.png]]


##### Powers of relation

![[Pasted image 20221022144517.png]]


### Properties of Relations


##### Reflexative Relations

R is reflexive iff (a,a) $\in$ R for every element a $\in$ A

$\forall x.$ ($x \in A \implies (x,x) \in R$)


##### Symmetric Relations

R is symmetric iff (b,a) $\in$ R whenever (a,b) $\in$ R for all a, b $\in$ A

$\forall x. \forall y. ((x,y) \in R \implies (y,x) \in R)$


##### Antisymmetric Relations

![[Pasted image 20221022180827.png]]


##### Transitive Relations

if whenever (a,b) $\in$ R and (b,c) $\in$ R, then (a,c) $\in$ R for all a, b, c $\in$ A

$\forall x, y, z. ((x,y) \in R \land (y,z) \in R \implies (x,z) \in R)$


##### Closures

if R is a relation on a set A, then the closure of R with respect to P, if it exists, is the relation S on A with property P that contains R and is a subset of every subset A X A containing R with property P.


### Equivalence Relations

R is called an equivalence relation if ir is reflective, symmetric and transitive

elements a and b related by an equivalence relation are called equivilent (a ~ b)


##### Equivalence classes

Let R be an equivalent relation to A. The set of all elements that are related to an element of A is called an equivalence class of a.

![[Pasted image 20221023124247.png]]

e.g: the equivalence class for 2 mod 4
$[2]r$ = {..., -6, -2, 2, 6, 10, ...} 

##### Partitions

![[Pasted image 20221025172632.png]]

A partition of a set S is a collection of disjoint nonempty subsets of S that have S as their union
![[Pasted image 20221025172726.png]]


##### Equivalence Relations and Partitions

![[Pasted image 20221025172840.png]]

![[Pasted image 20221025172852.png]]


### Partial Orderings

![[Pasted image 20221025173002.png]]

##### Hasse Diagrams

![[Pasted image 20221025173024.png]]

##### Constructing a Hasse Diagram

![[Pasted image 20221025173116.png]]

![[Pasted image 20221025173130.png]]

