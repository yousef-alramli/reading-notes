# Big O: Analysis of Algorithm Efficiency
Big-O is a metrics used to find algorithm complexity. Basically, Big-O notation signifies the relationship between the input to the algorithm and the steps required to execute the algorithm. It is denoted by a big "O" followed by opening and closing parenthesis.

Big O(oh) notation is used to describe the efficiency of an algorithm or function. This efficiency is evaluated based on 2 factors:

1. Running Time (also known as time efficiency / complexity)
The amount of time a function needs to complete.

1. Memory Space (also known as space efficiency / complexity)
The amount of memory resources a function uses to store data and instructions.

**In order to analyze limiting factors (time,space), we should consider 4 Key Areas for analysis:**

1. Input Size
1. Units of Measurement
1. Orders of Growth
1. Best Case, Worst Case, and Average Case

## Input Size
The O(n²) notation means that the runtime complexity of your algorithm is proportional to the square of input size. Let's say that the input size of your array is 3, then the runtime complexity of your algorithm will be increased by 9.

## Units of Measurement
*Big O doesn't measure a unit of time*. It expresses the runtime of the code in terms of input of size n. You can't accurately use a big O notation to compute runtime in milliseconds as this may vary per machine that you run the code on.

## Orders of Growth

An order of growth is a set of functions whose asymptotic growth behavior is considered equivalent. For example, 2n, 100n and n+1 belong to the same order of growth, which is written O(n) in Big-Oh notation and often called linear because every function in the set grows linearly with n.

 big O notation is used to classify algorithms according to how their run time or space requirements grow as the input size grows. The letter O is used because the growth rate of a function is also referred to as the order of the function.

## Worst Case, Best Case, Average Case

- **Worst Case**: The efficiency for the worst possible input of size n
- **Best Case**: The efficiency for the best possible input of size n
- **Average Case**: The efficiency for a “typical” or “random” input of size n.

## Review
Big O: The worst case analysis of algorithm efficiency.
Running Time: The amount of time required for an algorithm to complete.
Memory Space: The amount of memory resources required for an algorithm to complete.
Input Size: Represented by the variable n, the total size of values used as parameters in an algorithm.
Big Omega: The best case analysis of algorithm efficiency.
Big Theta: The typical or random case used for analysis of algorithm efficiency.

# Linked Lists
**A linked list** is a sequence of data elements, which are connected together via links. Each data element contains a connection to another data element in form of a pointer. Python does not have linked lists in its standard library

## What does it look like
![](https://miro.medium.com/max/953/1*elJncKhH_P9oQglfI1aVQA.png)


# What’s a Linked List
A linked list is a sequence of data elements, which are connected together via links. Each data element contains a connection to another data element in form of a pointer. Python does not have linked lists in its standard library. In this type of data structure there is only one link between any two data elements.

## Linear data structures
A Linear data structure have data elements arranged in sequential manner and each member element is connected to its previous and next element. 
## what is Big O
Big-O notation is a metrics used to find algorithm complexity. Basically, Big-O notation signifies the relationship between the input to the algorithm and the steps required to execute the algorithm. It is denoted by a big "O" followed by opening and closing parenthesis.

## Growing a linked list
**Linked lists** are like a lesser-known cousin of lists. They’re not as popular or as cool, and you might not even remember them from your algorithms class. But in the right context, they can really shine.

 *Each element of a linked list is called a node, and every node has two different fields:*
1. **Data** contains the value to be stored in the node.
1. **Next** contains a reference to the next node on the list.

