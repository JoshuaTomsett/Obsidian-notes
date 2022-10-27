[[ECM1415 Discrete Mathematics for Computer Science]]

10-Oct-2022

### Sets

- an unordered collection of objects
- objects are called elements, or memebers
- a $\in$ A denotes that a is an element of the set A
- if a is not a member of A then we write a $\notin$ A

![[Pasted image 20221014153548.png]]

Universal set ( $U$ ) : the set containing everything under consideration
Empty set ( $\emptyset$ ) : the set with no elements

#### Subsets

A is a subset of B - A $\subseteq$ B

A is a proper subset of B - A $\subset$ B

#### Cardinality

the number of elements in a set (n)
denoted by $|A|$ 

#### Power set

the set of all subsets
denoted by $\wp$(A)


### Set operations

==Union== - A $\cup$ B - { $x$ : $x \in A$ $\lor$ $x \in B$ }
![[Pasted image 20221014154742.png]]

==Intersection== - A $\cap$ B - { $x$ : $x \in A$ $\land$ $x \in B$ }
![[Pasted image 20221014154849.png]]

==Difference== - A $\setminus$ B - { $x$ : $x \in A$ $\land$ $x \notin B$ }
![[Pasted image 20221014155038.png]]

==Compliment== - $\overline A$ - { $x$ : $x \in U$ $\land$ $x \notin A$ }
![[Pasted image 20221014155051.png]]

### Set identities

![[Pasted image 20221014155343.png]]

#### Membership tables

![[Pasted image 20221014155445.png]]


### Recursively defined sets

Basis step : specifies the initial collection of elements

Recursive step : gives the rules for forming new elements in the set from those already know to be in the set

![[Pasted image 20221014155623.png]]

#### Structural induction

use to prove a property of the elements of a recursively defined set

![[Pasted image 20221014155805.png]]
