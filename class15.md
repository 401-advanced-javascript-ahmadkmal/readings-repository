# class 15 tree

## complete the sentence with the right words

..... is the individual item/data that makes up the data structure
..... is the first/top Node in the tree
....... The node that is positioned to the left of a root or node
....... The node that is positioned to the right of a root or node
....... in a tree is the link between a parent and child node
.......  is a node that does not contain any children
....... of a tree is determined by the number of edges from the root to the bottommost node

![tree](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/tree-example.png)
in the image above write :
Pre-order: root >> left >> right?
In-order: left >> root >> right?
Post-order: left >> right >> root?

## write the algorithm of pre order?

## which model od data structure used to do pre order?

## write the algorithm of in order?

## write the algorithm of post order?

## write the algorithm of breadthFirst?

## what is binary tree and the deferent between binary search tree?

## what is the big o of n for adding note in binary tree?

<!-- Node - 
Root - 
Left Child - 
Right Child - 
Edge - 
Leaf -
Height - 


Pre-order: A, B, D, E, C, F
In-order: D, B, E, A, F, C
Post-order: D, E, B, F, C, A

ALGORITHM preOrder(root)

  OUTPUT <-- root.value

  if root.left is not NULL
      preOrder(root.left)

  if root.right is not NULL
      preOrder(root.right)

 stack data structure 



 ALGORITHM inOrder(root)
// INPUT <-- root node
// OUTPUT <-- in-order output of tree node's values

    if root.left is not NULL
        inOrder(root.left)

    OUTPUT <-- root.value

    if root.right is not NULL
        inOrder(root.right)



ALGORITHM postOrder(root)
// INPUT <-- root node
// OUTPUT <-- post-order output of tree node's values

    if root.left is not NULL
        postOrder(root.left)

    if root.right is not NULL
        postOrder(root.right)

    OUTPUT <-- root.value

    ALGORITHM breadthFirst(root)
// INPUT  <-- root node
// OUTPUT <-- front node of queue to console

  Queue breadth <-- new Queue()
  breadth.enqueue(root)

  while breadth.peek()
    node front = breadth.dequeue()
    OUTPUT <-- front.value

    if front.left is not NULL
      breadth.enqueue(front.left)

    if front.right is not NULL
      breadth.enqueue(front.right)

binary tree the number doesn't have structure while the binary search tree always the right node is less than left and that hrp for finding the node 

big o of n -->