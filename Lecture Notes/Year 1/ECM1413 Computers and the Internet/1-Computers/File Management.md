[[ECM1413 Computers and the Internet]]

29-Sep-2022

A file : a named collection of related infomation that is recorded on secondary storage

File extensions help the OS determine how to interpret the file

### File Attributes (meta data)

![[Pasted image 20221013195253.png]]

### File Management in Linux

- an everything is a file approach
- a tree-like inode pointer structure

##### Linux file types

![[Pasted image 20221013195437.png]]

### Hard and Soft links

Hard links: point to a file via its inode
Soft links : points to file via filename
![[Pasted image 20221013195557.png]]

### File blocks

![[Pasted image 20221013195624.png]]

### The inode Pointer Structure

![[Pasted image 20221013195650.png]]

### Mass-Storage Structures

##### Magnetic Disks

![[Pasted image 20221013195904.png]]
![[Pasted image 20221013195914.png]]
![[Pasted image 20221013195925.png]]

##### Solid-State Disks

has no moving parts and stores data using flash memory
![[Pasted image 20221013200021.png]]
![[Pasted image 20221013200034.png]]
![[Pasted image 20221013200048.png]]
![[Pasted image 20221013200158.png]]
![[Pasted image 20221013200208.png]]

### Wear Levelling

Dynamic : new data is written to the least-recently-used block (to avoid using the same blocks)

Static : Peroidically move cold data to least-recently-used block

![[Pasted image 20221013200446.png]]
