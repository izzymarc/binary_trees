# Binary Trees

This repository contains exercises on implementing binary trees and performing various operations on them. The exercises progress from creating and inserting nodes to more complex operations like deleting the tree, checking properties (e.g., if a tree is full, perfect), and traversing the tree in different ways.

## Tasks

### 0. New node
Create a function that creates a binary tree node. Prototype: `binary_tree_t *binary_tree_node(binary_tree_t *parent, int value);` Your function must return a pointer to the new node, or NULL on failure.

### 1. Insert left
Write a function that inserts a node as the left-child of another node. Prototype: `binary_tree_t *binary_tree_insert_left(binary_tree_t *parent, int value);` If parent already has a left-child, the new node must take its place, and the old left-child must be set as the left-child of the new node.

### 2. Insert right
Function that inserts a node as the right-child of another node. Prototype: `binary_tree_t *binary_tree_insert_right(binary_tree_t *parent, int value);` If parent already has a right-child, the new node takes its place, and the old right-child is set as the right-child of the new node.

### 3. Delete
A function that deletes an entire binary tree. Prototype: `void binary_tree_delete(binary_tree_t *tree);` If tree is NULL, do nothing.

### 4. Is leaf
Check if a node is a leaf. Prototype: `int binary_tree_is_leaf(const binary_tree_t *node);` Returns 1 if node is a leaf, otherwise 0. If node is NULL, return 0.

### 5. Is root
Check if a given node is a root. Prototype: `int binary_tree_is_root(const binary_tree_t *node);` Returns 1 if node is a root, otherwise 0. If node is NULL, return 0.

### 6. Pre-order traversal
Function that goes through a binary tree using pre-order traversal. Prototype: `void binary_tree_preorder(const binary_tree_t *tree, void (*func)(int));`

### 7. In-order traversal
Traverse a binary tree using in-order traversal. Prototype: `void binary_tree_inorder(const binary_tree_t *tree, void (*func)(int));`

### 8. Post-order traversal
Traverse a binary tree using post-order traversal. Prototype: `void binary_tree_postorder(const binary_tree_t *tree, void (*func)(int));`

### 9. Height
Measure the height of a binary tree. Prototype: `size_t binary_tree_height(const binary_tree_t *tree);` If tree is NULL, your function must return 0.

### 10. Depth
Measure the depth of a node in a binary tree. Prototype: `size_t binary_tree_depth(const binary_tree_t *tree);` If tree is NULL, your function must return 0.

### 11. Size
Measure the size of a binary tree. Prototype: `size_t binary_tree_size(const binary_tree_t *tree);` If tree is NULL, the function must return 0.

### 12. Leaves
Count the leaves in a binary tree. Prototype: `size_t binary_tree_leaves(const binary_tree_t *tree);` If tree is NULL, the function must return 0. A NULL pointer is not a leaf.

### 13. Nodes
Count the nodes with at least 1 child in a binary tree. Prototype: `size_t binary_tree_nodes(const binary_tree_t *tree);` If tree is NULL, the function must return 0. A NULL pointer is not a node.

### 14. Balance factor
Measure the balance factor of a binary tree. Prototype: `int binary_tree_balance(const binary_tree_t *tree);` If tree is NULL, return 0.

### 15. Is full
Check if a binary tree is full. Prototype: `int binary_tree_is_full(const binary_tree_t *tree);` If tree is NULL, your function must return 0.

### 16. Is perfect
Check if a binary tree is perfect. Prototype: `int binary_tree_is_perfect(const binary_tree_t *tree);` If tree is NULL, your function must return 0.

### 17. Sibling
Find the sibling of a node. Prototype: `binary_tree_t *binary_tree_sibling(binary_tree_t *node);` If node is NULL or the parent is NULL, return NULL. If node has no sibling, return NULL.

### 18. Uncle
Find the uncle of a node. Prototype: `binary_tree_t *binary_tree_uncle(binary_tree_t *node);` If node is NULL, return NULL. If node has no uncle, return NULL.

## Compilation and Examples
To compile the code for each task, use gcc with the options `-Wall -Wextra -Werror -