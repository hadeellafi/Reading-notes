# Stacks and Queues

## What is a Stack?

A stack is a data structure that consists of **nodes**. Each **node** references the next node in the stack but does not reference its previous.

An analogy to understand this concept is to imagine a box representing a stack that contains a number of books. In this analogy, you cannot access the first book in the box without first removing the last books that were added.

<div style="text-align: center;">
<img src="../assets/stack.jpg" alt="Image" width="50%" >
</div>

## Stack Concepts

From the books example, we can figure out the following stack concepts:

- **FILO** (First In Last Out): The first book we put in will be the last one to be taken out.

- **LIFO** (Last In First Out): The last book added will be the first one to be taken out.

## Common Terminology for a Stack

- **Push**: Adding an element to the stack.
- **Pop**: Removing an element from the stack.
- **Top**: Refers to the top of the stack, which is the last element added to the stack.
- **Peek**: Viewing the value of the top node in the stack without altering the stack.
- **IsEmpty**: A condition that returns true when the stack is empty; otherwise, it returns false.

The difference between "top" and "peek" is that "top" represents the actual position of the most recent element in the stack, while "peek" is an operation that allows you to observe the value of the top element without altering the stack.

## What is a Queue?

A queue is a data structure that follows a **FIFO** (First In First Out) order. It operates similarly to a line of people waiting for a service, where the first person who joins the line is the first one to be served.

<div style="text-align: center;">
<img src="../assets/queue.jpg" alt="Image" width="50%" >
</div>

## Common Terminology for a Queue

Queues follow these concepts:

- **FIFO** (First In First Out): The first item in the queue will be the first item out of the queue.

- **LILO** (Last In Last Out): The last item in the queue will be the last item out of the queue.

## Common Terminology for a queue

- **Enqueue**: Adding  to the queue.
- **Dequeue**: Removing from the queue.
- **Front**: Refers to the front/first node of the queue.
- **Rear**: Refers to the rear/last node of the queue.
- **Peek**: Viewing the value of the front node in the queue.
- **IsEmpty**: Returns true when the queue is empty; otherwise, it returns false.
