# Read 15 - Tree
># Tree
## What is a Tree data structure ?


### A tree is non-linear and a hierarchical data structure consisting of a collection of nodes such that each node of the tree stores a value and a list of references to other nodes (the “children”).

### This data structure is a specialized method to organize and store data in the computer to be used more effectively. It consists of a central node, structural nodes, and sub-nodes, which are connected via edges. We can also say that tree data structure has roots, branches, and leaves connected with one another. 

<img src="https://media.geeksforgeeks.org/wp-content/cdn-uploads/binary-tree-to-DLL.png">

## Why Tree is considered a non-linear data structure?

### The data in a tree are not stored in a sequential manner i.e, they are not stored linearly. Instead, they are arranged on multiple levels or we can say it is a hierarchical structure. For this reason, the tree is considered to be a non-linear data structure.

## Basic Terminologies In Tree Data Structure:

* ##  Parent Node: 
###  The node which is a predecessor of a node is called the parent node of that node. `{2}` is the parent node of `{6, 7}`.

* ## Child Node: 
###  The node which is the immediate successor of a node is called the child node of that node. Examples: `{6, 7}` are the child nodes of `{2}`.

* ## Root Node: 
###  The topmost node of a tree or the node which does not have any parent node is called the root node. `{1}` is the root node of the tree. A non-empty tree must contain exactly one root node and exactly one path from the root to all other nodes of the tree.

* ## Leaf Node or External Node: 
###  The nodes which do not have any child nodes are called leaf nodes. `{6, 14, 8, 9, 15, 16, 4, 11, 12, 17, 18, 19}` are the leaf nodes of the tree.

* ## Ancestor of a Node: 
###  Any predecessor nodes on the path of the root to that node are called Ancestors of that node. `{1, 2}` are the ancestor nodes of the node `{7}`.

* ## Descendant: 
###  Any successor node on the path from the leaf node to that node. `{7, 14}` are the descendants of the node.`{2}`.

* ## Sibling: 
###  Children of the same parent node are called siblings. `{8, 9, 10}` are called siblings.

* ## Level of a node: 
###  The count of edges on the path from the root node to that node. The root node has level 0.

* ## Internal node: 
###  A node with at least one child is called Internal Node.

* ## Neighbour of a Node: 
###  Parent or child nodes of that node are called neighbors of that node.

* ## Subtree: 
###  Any node of the tree along with its descendant.


## Properties of a Tree:

* ## Number of edges: 
###  An edge can be defined as the connection between two nodes. If a tree has N nodes then it will have (N-1) edges. There is only one path from each node to any other node of the tree.

* ## Depth of a node: 
###  The depth of a node is defined as the length of the path from the root to that node. Each edge adds 1 unit of length to the path. So, it can also be defined as the number of edges in the path from the root of the tree to the node.

* ## Height of a node: 
###  The height of a node can be defined as the length of the longest path from the node to a leaf node of the tree.

* ## Height of the Tree: 
###  The height of a tree is the length of the longest path from the root of the tree to a leaf node of the tree.

* ## Degree of a Node: 
###  The total count of subtrees attached to that node is called the degree of the node. The degree of a leaf node must be 0. The degree of a tree is the maximum degree of a node among all the nodes in the tree.

# Example of Tree data structure

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20211127152300/imi-300x258.png">

* Node A is the root node
* B is the parent of D and E
* D and E are the siblings
* D, E, F and G are the leaf nodes
* A and B are the ancestors of E

># Types of Tree data structures : 
## 1. General tree

### A general tree data structure has no restriction on the number of nodes. It means that a parent node can have any number of child nodes.  

## 2. Binary tree  

### A node of a binary tree can have a maximum of two child nodes. In the given tree diagram, node B, D, and F are left children, while E, C, and G are the right children.  

## 3. Balanced tree

### If the height of the left sub-tree and the right sub-tree is equal or differs at most by 1, the tree is known as a balanced tree.  

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20220614001043/upload.png">

## 4. Binary search tree

### As the name implies, binary search trees are used for various searching and sorting algorithms. The examples include AVL tree and red-black tree. It is a non-linear data structure. It shows that the value of the left node is less than its parent, while the value of the right node is greater than its parent.


># Applications of Tree data structure:
## 1. Spanning trees: It is the shortest path tree used in the routers to direct the packets to the destination.  

## 2. Binary Search Tree: It is a type of tree data structure that helps in maintaining a sorted stream of data.  

## 3. Storing hierarchical data: Tree data structures are used to store the hierarchical data, which means data is arranged in the form of order.  

## 4. Syntax tree: The syntax tree represents the structure of the program’s source code, which is used in compilers.  

## 5. Trie: It is a fast and efficient way for dynamic spell checking. It is also used for locating specific keys from within a set.  

## 6. Heap: It is also a tree data structure that can be represented in a form of an array. It is used to implement priority queues.  
Footer
© 2022 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
