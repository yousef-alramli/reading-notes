# TDD with Python
## TTD 
Test-driven development (TDD) is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases.

## Unit tests and TDD
 is writing many small tests that each test one very simple function or object behavior. TDD is a thinking process that results in unit tests, and “thinkiHow memory is allocated to different function calls in recursion?ng in tests” tends to result in more fine-grained and comprehensive testing, and an easier-to-extend software design.

## structure
 A convention widely used is the AAA:
- **Arrange**, Act and Assert.
Arrange: you need to organize the data needed to execute that piece of code (input);
- **Act**: here you will execute the code being tested (exercise the behaviour);
- **Assert**: after executing the code, you will check if the result (output) is the same as you were expecting.

## tdd cycle
TDD cycle defines
1. Write a test
1. Make it pass.
1. Change the code to make it right i.e.
Refactor.


# If name equals main
## What does the if __ name__ == “__ main__”: do?
is used to execute some code only if the file was run directly, and not imported.

A module is a file containing Python definitions and statements. The file name is the module name with the suffix .py appended. 

Advantages : 

1. Every Python module has it’s __ name__ defined and if this is ‘__ main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.
1. If you import this script as a module in another script, the __ name__ is set to the name of the script/module.
1. Python files can act as either reusable modules, or as standalone programs.
if __ name__ == “main”: is used to execute some code only if the file was run directly, and not imported.

# Recursion
Recursion is the process of defining a problem (or the solution to a problem) in terms of (a simpler version of) itself.

## A Mathematical Interpretation
Let us consider a problem that a programmer have to determine the sum of first n natural numbers, there are several ways of doing that but the simplest approach is simply add the numbers starting from 1 to n. So the function simply looks like,



    approach(1) – Simply adding one by one
    
    f(n) = 1 + 2 + 3 +……..+ n

but there is another mathematical approach of representing this,

    approach(2) – Recursive adding 

    f(n) = 1                  n=1

    f(n) = n + f(n-1)    n>1

There is a simple difference between the approach (1) and approach(2) and that is in approach(2) the function “ f( ) ” itself is being called inside the function, so this phenomenon is named as recursion and the function containing recursion is called recursive function, at the end this is a great tool in the hand of the programmers to code some problems in a lot easier and efficient way.


**How a particular problem is solved using recursion?**
The idea is to represent a problem in terms of one or more smaller problems, and add one or more base conditions that stop the recursion. 


**Why Stack Overflow error occurs in recursion?**
The most-common cause of stack overflow is excessively deep or infinite recursion, in which a function calls itself so many times that the space needed to store the variables and information associated with each call is more than can fit on the stack.



**How memory is allocated to different function calls in recursion?** 
When any function is called from main(), the memory is allocated to it on the stack. A recursive function calls itself, the memory for a called function is allocated on top of memory allocated to calling function and different copy of local variables is created for each function call.


**What are the disadvantages of recursive programming over iterative programming?** 
Note that both recursive and iterative programs have the same problem-solving powers, i.e., every recursive program can be written iteratively and vice versa is also true. The recursive program has greater space requirements than iterative program as all functions will remain in the stack until the base case is reached. It also has greater time requirements because of function calls and returns overhead.