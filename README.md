# Binary Search Trees

---

### 06/12/2019

## Trees

Can be thought of as linked lists, but without the constraint that each node only points to one other node. A tree node can point to multiple other nodes in the tree. Linked Lists themselves count as trees.

## Binary Tree

at most a single node can point to 2 nodes.

For any given node, all values in the left subtree are less than the value at the given node.

Conversely, all values in the right subtree are greater than or equal to the value at the given node.

Data doesn't need to be sorted

Provides order to unsorted data in a way

              x

         |           |

         X          X

       |      |     |    |

       X     X   X   X

    # Example Binary Search Tree Class
    class BinarySearchTree:
        self.value = value
        self.left = left_subtree
        self.right = right_subtree

Check for value in BST : bst.contains(10)

1. Compare initial value to root of the tree
2. left if lower right if higher and then compare with next node
3. repeat again
4. if found return True

Pros : Searching for an element in a binary search tree is significantly more efficient than searching through an array or linked list

Cons : it is not as efficient to insert into a binary search tree.  performance of a binary search tree depends quite a lot on whether the tree is 'balanced' or not. 

## Ternary Tree

at most single node can point to 3 nodes

## 4-ary Tree

at most single node can point to 4 nodes

Root : The topmost node in the tree

Child : node directly connected to another node when moving away from the root node

Parent : A node directly connected to another node when moving towards the root node

Siblings : Nodes that share the same parent re considered siblings

Leaf : node that does not have any children of it's own.