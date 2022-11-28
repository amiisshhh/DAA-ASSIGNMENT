# DAA-ASSIGNMENT


# Name : AMISH SINGH

# Roll no: A-35 (V SEM)

# DAA Assignment 1

# Aim : Give an application and its implementation to demonstrate the rotations operations RB [Red-Black trees

# Theory :

It a Binary Search Tree [BST]
 1) The Root node of the tree is black.
 2) If leaf node is Null then it is considered as Black. [In some operations
Null leaf node is also used, hence colouring is important]
 3) If node is “Red” then its children will be “Black”
 4) Every path from a node to a descendant leaf, will contain same
number of black nodes.
 5) Black Height: The number of black nodes in the path from a node, but not including node is called as “Black-height” bh(x)
 6) Rotation: It is an operation required to balance the tree height, and it will be always in opposite direction of insertion.
 7) Initial colour of any new node is “RED”
 8) Recoloring operation allows change of colour [RED-BLACK-RED]
 9) Generally Red-Black recoloring is more required in Tree balancing
operation.
 10) Red nodes can only have “Black” children.


# Rules for Red-Black Trees :
Every node has a color either red or black.
The root of the tree is always black.
There are no two adjacent red nodes (A red node cannot have a red parent or red child).
Every path from a node (including root) to any of its descendants NULL nodes has the same number of black nodes.
All leaf nodes are black nodes.
![REDBLACK](https://user-images.githubusercontent.com/112940949/203837420-9a164ce7-ab15-4ac2-b7ab-bb673260b2b1.jpg)



# Rotations in Red Black Trees :
In rotation operation, the positions of the nodes of a subtree are interchanged. Rotation operation is used for maintaining the properties of a red-black tree when they are violated by other operations such as insertion and deletion.
# There are two major types of roations:
1.Left Rotation
2.Right Roation
![RB_Rotation](https://user-images.githubusercontent.com/112940949/203839934-28c59358-68db-4bc8-a9b6-db8f08648431.jpg)

# ALGORITHMS:
## LEFT ROTATE (T, x)
 1. y ← right [x]
 1. y ← right [x]
 2. right [x] ← left [y]
 3. p [left[y]] ← x
 4. p[y] ← p[x]
 5. If p[x] = nil [T]
   then root [T] ← y
    else if x = left [p[x]] 									
      then left [p[x]] ← y
    else right [p[x]] ← y
 6. left [y] ← x.
 7. p [x] ← y.

## RIGHT ROTATE(T,x)
LEFT ROTATE (T, x)
 1. y ← left [x]
 1. y ← left [x]
 2. left [x] ← right [y]
 3. p [right[y]] ← x
 4. p[y] ← p[x]
 5. If p[x] = nil [T]
   then root [T] ← y
    else if x = left [p[x]] 									
      then left [p[x]] ← y
    else right [p[x]] ← y
 6. right [y] ← x.
 7. p [x] ← y.

## INSERTION ALGORITHM:
RB-INSERT (T, z)
 1. y ← nil [T]
 2. x ← root [T]
 3. while x ≠ NIL [T]
 4. do y ← x
 5. if key [z] < key [x]
 6. then x  ← left [x]
 7. else x ←  right [x]
 8. p [z] ← y
 9. if y = nil [T]
 10. then root [T] ← z
 11. else if key [z] < key [y]
 12. then left [y] ← z
 13. else right [y] ← z
 14. left [z] ← nil [T]
 15. right [z] ← nil [T]
 16. color [z] ← RED
 17. RB-INSERT-FIXUP (T, z)

EXAMPLE:

![INsertion](https://user-images.githubusercontent.com/112940949/203843034-65144ed5-9dc9-4423-b2a4-de08be503be7.jpg)



## DELETION ALGORITHM:
RB-DELETE (T, z)
 1. if left [z] = nil [T] or right [z] = nil [T]
 2. then y ← z
 3. else y ← TREE-SUCCESSOR (z)
 4. if left [y] ≠ nil [T]
 5. then x ← left [y]
 6. else x ← right [y]
 7. p [x] ←  p [y]
 8. if p[y] = nil [T]
 9. then root [T]  ← x
 10. else if y = left [p[y]]
 11. then left [p[y]] ← x
 12. else right [p[y]] ← x
 13. if y≠ z
 14. then key [z] ← key [y]
 15. copy y's satellite data into z
 16. if color [y] = BLACK
 17. then RB-delete-FIXUP (T, x)
 18. return y



 EXAMPLE:

![Deletion](https://user-images.githubusercontent.com/112940949/203843054-aa747962-357a-4380-aa91-0d5cc8e68507.jpg)



# Applications of Red-Black Trees :
1. To implement finite maps.
2. Machine Learning K-mean clustering algorithm for reducing Time Complexity.
3. To implement Standard Template Libraries (STL) in C++: multiset, map, multimap.
4. MySQL also uses Red-Black Tree indexing to reduce the searching and insertion time.
5. To implement Java packages: TreeMap and TreeSet.
6. In Linux Kernel.


## Some References and ideas for implementation taken from:
1. http://www.mbchandak.com/
2. https://www.geeksforgeeks.org/

