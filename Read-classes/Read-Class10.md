# Stacks and Queues

- **Stacks** and **queues** are two types of collections in C# that store elements in a specific order. A stack follows the **last-in**, **first-out (LIFO)** principle, meaning that the last element added to the stack is the first one to be removed. A ***queue*** follows the **first-in**, **first-out (FIFO)** principle, meaning that the first element added to the queue is the first one to be removed.

- To use stacks and queues in C#, you need to import the `System.Collections.Generic` namespace and create an instance of the `Stack<T>` or `Queue<T>` class, where `T`is the type of elements you want to store. For example, if you want to store integers, you can write:

      Stack<int> myStack = new Stack<int>();
      Queue<int> myQueue = new Queue<int>();

- To add elements to a stack or a queue, you use the `Push` or `Enqueue` method, respectively. For example:

      myStack.Push(10); // adds 10 to the top of the stack
      myQueue.Enqueue(10); // adds 10 to the end of the queue

- To remove and return elements from a stack or a queue, you use the `Pop` or `Dequeue` method, respectively. For example:

      int x = myStack.Pop(); // removes and returns the top element of the stack
      int y = myQueue.Dequeue(); // removes and returns the first element of the queue

- To access but not remove elements from a stack or a queue, you use the `Peek` method. For example:

      int x = myStack.Peek(); // returns the top element of the stack without removing it
      int y = myQueue.Peek(); // returns the first element of the queue without removing it

- To check if a stack or a queue is empty, you can use the `Count` property. For example:

      if (myStack.Count == 0) // checks if the stack is empty
      if (myQueue.Count == 0) // checks if the queue is empty

- To clear all elements from a stack or a queue, you can use the `Clear` method. For example:

      myStack.Clear(); // removes all elements from the stack
       myQueue.Clear(); // removes all elements from the queue

To iterate over a stack or a queue, you can use a `foreach` loop. For example:

    foreach (int item in myStack) // loops through each item in the stack
    foreach (int item in myQueue) // loops through each item in the queue
