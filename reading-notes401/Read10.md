# Stacks and Queues
**Stacks** and **queues** are simple data structures that allow us to store and retrieve data sequentially. In a stack, the last item we enter is the first to come out. In a queue, the first item we enter is the first come out. We can add items to a stack using the push operation and retrieve items using the pop operation.

## Stack
Common terminology for a stack is:

1. Push - Nodes or items that are put into the stack are pushed
1. Pop - Nodes or items that are removed from the stack are popped. When you attempt topop an empty stack an exception will be raised.
1. Top - This is the top of the stack.
1. Peek - When you peek you will view the value of the top Node in the stack. When youattempt to peek an empty stack an exception will be raised.
1. IsEmpty - returns true when stack is empty otherwise returns false.

**Stacks concepts:**
- FILO
First In Last Out  
This means that the first item added in the stack will be the last item popped out of the stack.

- LIFO
Last In First Out  
This means that the last item added to the stack will be the first item popped out of the stack.

- Stack Visualization
Here’s an example of what a stack looks like. As you can see, the topmost item is denoted as the top. When you push something to the stack, it becomes the new top. When you pop something from the stack, you pop the current top and set the next top as top.next.

- Push O(1)
Pushing a Node onto a stack will always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.

- Pop O(1)
Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user.

- Peek O(1)
When conducting a peek, you will only be inspecting the top Node of the stack.  
Typically, you would check isEmpty before conducting a peek. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.

- IsEmpty O(1)
Here is the pseudocode for isEmpty

## Queue

Common terminology for a queue is

1. Enqueue - Nodes or items that are added to the queue.
1. Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
1. Front - This is the front/first Node of the queue.
1. Rear - This is the rear/last Node of the queue.
1. Peek - When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised.
1. IsEmpty - returns true when queue is empty otherwise returns false.

**Queues concepts:**

- FIFO
First In First Out  
This means that the first item in the queue will be the first item out of the queue.

- LILO
Last In Last Out  
This means that the last item in the queue will be the last item out of the queue.

- Queue Visualization

- Enqueue O(1)
When you add an item to a queue, you use the enqueue action. This is done with an O(1) operation in time because it does not matter how many other items live in the queue (n); it takes the same amount of time to perform the operation.