[[ECM1415 Discrete Mathematics for Computer Science]]

16-Nov-2022


### Basic Counting Principles

##### The Product Rule

A procedure can be broken down into a sequence of two tasks. There are $n_1$ ways to do the first task and $n_2$ ways to do the second task. Then there are $n_1 ∗ n_2$ ways to do the procedure

##### The Sum Rule

If a task can be done either in one of n1 ways or in one of $n_2$, where none of the set of $n_1$ ways is the same as any of the $n_2$ ways, then there are $n_1 + n_2$ ways to do the task

##### The Subtraction Rule

If a task can be done either in one of $n_1$ ways or in one of $n_2$, then the total number of ways to do the task is $n_1 + n_2$ minus the number of ways to do the task that are common to the two different ways

##### The Division Rule

There are $n/d$ ways to do a task if it can be done using a procedure that can be carried out in $n$ ways, and for every way $w$, exactly $d$ of the $n$ ways correspond to way $w$.


### The Pigeonhole Principle

If  k is a positive integer and k+1 objects are placed into k boxes, then at least one box contains two or more objects

![[Pasted image 20221121154611.png]]

##### Generalized Pigeonhole Principle

![[Pasted image 20221121154647.png]]


### Permutations

A permutation of a set of distinct objects is an ordered arrangement of those objects

An ordered arrangement of r elements of a set is called an `r-permutation`
The number of r-permutations of a set with n elements is denoted $P(n,r)$

Example: let S = {1, 2, 3}

the 2-permutations of S = 1,2; 1,3; 2,1; 2,3; 3,1; 3,2
Hence $P(3,2) = 6$

![[Pasted image 20221121155354.png]]
![[Pasted image 20221121155433.png]]


### Combinations

An r-combination of elements of a set is an unordered selection of r elements from the set

- An r-combination is simply a subset of the set with r elements
- The number of r-combinations of a set with n distinct elements is denoted by $C(n,r)$
![[Pasted image 20221121155708.png]]

![[Pasted image 20221121155722.png]]

![[Pasted image 20221121155739.png]]

![[Pasted image 20221121155749.png]]

![[Pasted image 20221121155757.png]]

![[Pasted image 20221121155817.png]]

##### Combinational Proofs

![[Pasted image 20221121155846.png]]

![[Pasted image 20221121155952.png]]
![[Pasted image 20221121160003.png]]


### Generalized Permutations

##### Permuations with repetition

The number of r-permutations of a set of n objects with repetition allowed is $n^r$

Proof:
- There are n ways to select an element of the set for each of the r positions in the r-permutation when repetition is allowed
- Hence, by the product rule there are $n^r$ r-permutations with repetition

![[Pasted image 20221121160404.png]]

##### Combinations with repetition

![[Pasted image 20221121160527.png]]
![[Pasted image 20221121160537.png]]

##### Summary

![[Pasted image 20221121160556.png]]
