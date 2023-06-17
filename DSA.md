# Data Structures and Algorithms

### 🤔 why this topic matters as it relates to what I'am studying in this module? 

- Data structures are being used in almost every program or software system that has been developed. Moreover, data structures come under the fundamentals of Computer Science 🖥️ and Software Engineering. Hence as developers, we must have good knowledge about data structures.
[READ MORE](https://towardsdatascience.com/8-common-data-structures-every-programmer-must-know-171acf6a1a42)

---

### What is 1 of the more important things you should consider when deciding which data structure is best suited to solve a particular problem?

I will mention here the three most important things to consider when deciding which data structure is best suited to solve a particular problem:

1. **Time** and **space complexity** of the data structure.
2. **Type** and **nature** of the ***data*** I'am dealing with.
3. **Operations** and **functionalities** that I need to perform on the ***data***.
[READ MORE](https://www.geeksforgeeks.org/learn-data-structures-and-algorithms-dsa-tutorial/)

 ---

### understanding the ***Big O*** :

***Big O notation*** is a way to describe how fast a function grows. It’s often used in computer science to compare the efficiency of different algorithms. For example, if an algorithm has a ***Big O notation*** of **O(n)**, it means that its running time grows linearly with the size of the input.

 ---

### How can we ensure that we’ll avoid an infinite recursive call stack?

- We need to make sure that the function will eventually stop calling itself. This is done by defining a **base case**, which is a condition that stops the recursion when it is met.

- By using **tail recursion** and it is a technique where the recursive call is the last operation performed in the function. This allows the compiler to optimize the recursion and avoid creating a new stack frame for each recursive call, which can help prevent an infinite recursive call stack.

