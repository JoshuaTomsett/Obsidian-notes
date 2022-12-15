[[ECM1415 Discrete Mathematics for Computer Science]]

07-Dec-2022


### Introduction to Trees

A tree is a connected, undirected graph with no simple circuits

- A forest is a graph that has no simple circuits, but is not connected
- Each of the connected components in a forest is a tree

![[Pasted image 20221215120038.png]]


### Rooted Trees

A rooted tree is a tree in which one vertex has been designated as the root and every edge is directed away from the root

![[Pasted image 20221215120146.png]]


### Terminology

If v is a vertex of a rooted tree other than the root, the parent of v is the unique vertex u such that there is a directed edge from u to v

- When u is a parent of v, v is called a child of u
- Vertices with the same parent are called siblings
- A vertex with no children is called a leaf
- Vertices that have children are called internal vertices

The ancestors of a vertex are the vertices in the path from the root to the vertex, excluding the vertex itself and including the root. The descendants of a vertex v are those vertices that have v as an ancestor


### m-ary Rooted Trees

A rooted tree is called an m-ary tree if every internal vertex has no more than m children

- It is called a full m-ary tree if every internal vertex has exactly m children
- An m-ary tree with $m=2$ is called a binary tree

![[Pasted image 20221215121943.png]]


### Ordered Rooted Trees

An ordered rooted tree is a rooted tree where the children of each internal vertex are ordered

A binary tree is an ordered rooted tree where each internal vertex has at most two children
- If an internal vertex of a binary tree has two children, the first is called the left child and the second is called the right child
- The tree rooted at the left child is called the left subtree of this vertex


### Properties

![[Pasted image 20221215122346.png]]

#### Counting Vertices in Full m-ary Trees

![[Pasted image 20221215122436.png]]

![[Pasted image 20221215122447.png]]

#### Level of Vertices and Height of Trees

The level of a vertex v in a rooted tree is the length of the path from the root to v

The height of a rooted tree is the maximum of the levels of the vertices

![[Pasted image 20221215122642.png]]


### Tree Traversal

#### Preorder Traversal

![[Pasted image 20221215122751.png]]

#### Inorder Traversal

![[Pasted image 20221215122808.png]]

#### Postorder Traversal

![[Pasted image 20221215122826.png]]


### Spanning Trees

![[Pasted image 20221215122936.png]]
![[Pasted image 20221215122952.png]]


#### Correctedness

![[Pasted image 20221215123021.png]]

