# class 10

## Stacks 

A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.

Common terminology for a stack is

Push - Nodes or items that are put into the stack are pushed
Pop - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
Top - This is the top of the stack.
Peek - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised.
IsEmpty - returns true when stack is empty otherwise returns false.

### Stacks follow these concepts

#### FILO

First In Last Out

This means that the first item added in the stack will be the last item popped out of the stack.

#### LIFO

Last In First Out

This means that the last item added to the stack will be the first item popped out of the stack.

### Push O(1)

ALOGORITHM push(value)
// INPUT <-- value to add, wrapped in Node internally
// OUTPUT <-- none
   node = new Node(value)
   node.next <-- Top
   top <-- Node

### Pop O(1)

ALGORITHM pop()
// INPUT <-- No input
// OUTPUT <-- value of top Node in stack
// EXCEPTION if stack is empty

   Node temp <-- top
   top <-- top.next
   temp.next <-- null
   return temp.value

### peek

it will return the head to use data


ALGORITHM peek()
// INPUT <-- none
// OUTPUT <-- value of top Node in stack
// EXCEPTION if stack is empty

   return top.value


### IsEmpty O(1)

ALGORITHM isEmpty()
// INPUT <-- none
// OUTPUT <-- boolean

return top = NULL

## Queues

it away to store a data but the it seems like array 

### add

ALGORITHM enqueue(value)
// INPUT <-- value to add to queue (will be wrapped in Node internally)
// OUTPUT <-- none
   node = new Node(value)
   rear.next <-- node
   rear <-- node

### dequeue

ALGORITHM dequeue()
// INPUT <-- none
// OUTPUT <-- value of the removed Node
// EXCEPTION if queue is empty

   Node temp <-- front
   front <-- front.next
   temp.next <-- null

   return temp.value

### Peek

ALGORITHM peek()
// INPUT <-- none
// OUTPUT <-- value of the front Node in Queue
// EXCEPTION if Queue is empty

   return front.value


### IsEmpty O(1)

ALGORITHM isEmpty()
// INPUT <-- none
// OUTPUT <-- boolean

return front = NULL