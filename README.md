# DAA-ASSIGNMENT


# Name : AMISH SINGH

# Roll no: A-35 (V SEM)

# DAA Assignment 1

# Aim : Give an application and its implementation to demonstrate the rotations operations RB [Red-Black trees

# Theory :

It a Binary Search Tree [BST]
• The Root node of the tree is black.
• If leaf node is Null then it is considered as Black. [In some operations
Null leaf node is also used, hence colouring is important]
• If node is “Red” then its children will be “Black”
• Every path from a node to a descendant leaf, will contain same
number of black nodes.
• Black Height: The number of black nodes in the path from a node, but not including node is called as “Black-height” bh(x).
• Rotation: It is an operation required to balance the tree height, and it will be always in opposite direction of insertion.
• Initial colour of any new node is “RED”
• Recoloring operation allows change of colour [RED-BLACK-RED]
• Generally Red-Black recoloring is more required in Tree balancing
operation.
• Red nodes can only have “Black” children.


# Rules for Red-Black Trees :
Every node has a color either red or black.
The root of the tree is always black.
There are no two adjacent red nodes (A red node cannot have a red parent or red child).
Every path from a node (including root) to any of its descendants NULL nodes has the same number of black nodes.
All leaf nodes are black nodes.
![IMG_20221124_223300](https://user-images.githubusercontent.com/112940949/203836907-0a0d4c27-579a-4e83-8d05-d908f5a7ee3d.jpg)


# Rotations in Red Black Trees :
In rotation operation, the positions of the nodes of a subtree are interchanged. Rotation operation is used for maintaining the properties of a red-black tree when they are violated by other operations such as insertion and deletion.

