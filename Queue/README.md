# Queue
Queue is also an abstract data type or a linear data structure, in which the first element is inserted from one 
end called REAR(also called tail), and the deletion of exisiting element takes place from the other end called as 
FRONT(also called head). This makes queue as FIFO data structure, which means that element inserted first will also be removed first.

The process to add an element into queue is called Enqueue and the process of removal of an element from queue is called Dequeue.
<p align="center">
<img src="http://www.studytonight.com/data-structures/images/introduction-to-queue.png"?raw="true">
</p>

### Basic features of Queue
* Like Stack, Queue is also an ordered list of elements of similar data types.
* Queue is a FIFO( First in First Out ) structure.
* Once a new element is inserted into the Queue, all the elements inserted before the new element in the queue must be removed, to remove the new element.
* peek( ) function is oftenly used to return the value of first element without dequeuing it.

### Applications of Queue
Queue, as the name suggests is used whenever we need to have any group of objects in an order in which the first one coming in, also gets out first while the others wait for there turn, like in the following scenarios :

* Serving requests on a single shared resource, like a printer, CPU task scheduling etc.
* In real life, Call Center phone systems will use Queues, to hold people calling them in an order, until a service representative is free.
* Handling of interrupts in real-time systems. The interrupts are handled in the same order as they arrive, First come first served.

### Implementation of Queue
Queue can be implemented using an Array, Stack or Linked List. The easiest way of implementing a queue is by using an Array. 
Initially the head(FRONT) and the tail(REAR) of the queue points at the first index of the array 
(starting the index of array from 0). As we add elements to the queue, the tail keeps on moving ahead, 
always pointing to the position where the next element will be inserted, while the head remains at the first index.
<p align="center">
<img src="http://www.studytonight.com/data-structures/images/implementation-of-queue.png"?raw="true">
</p>
When we remove element from Queue, we can follow two possible approaches (mentioned [A] and [B] in above diagram). 
In [A] approach, we remove the element at head position, and then one by one move all the other elements on position forward. 
In approach [B] we remove the element from head position and then move head to the next position.

In approach [A] there is an overhead of shifting the elements one position forward every time we remove the first element. 
In approach [B] there is no such overhead, but whener we move head one position ahead, after removal of first element, 
the size on Queue is reduced by one space each time.

### Collected From
www.studytonight.com/
