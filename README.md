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


