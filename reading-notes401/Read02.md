# In Tests We Trust — TDD with Python
Some time ago, when I was beginning my career as a programmer, I heard other programmers talking about two things: refactoring and unit tests. To be honest, they just talk about refactoring to explain why this practice should be avoided (and how scared they were to do it) and about unit tests to say they are too expensive to begin with, that they spend a lot of time, etc. Unit tests did sound like a utopian dream.
## Unit tests and TDD
Probably there are million of blog posts about this subject. But let’s talk just a bit about it on my point of view!
Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.
## The freela
Imagine that a client has a website and through it he receives a lot of contacts from potential customers. After a while he realized that it is important for the business to identify the profile of consumer: age, gender, job and so on. But the website just receive the name and the email.
## Baby Steps
The API is pretty straightforward and your work was almost done. But with TDD we need to think about tests first. And to be ok with the possibility of the beginning to be hard sometimes — and it’s totally fine. Really.
## Important aspects about the unit test
There are some details to pay attention. The first one is the test name. The tests can be considered as your alive documentation. We need to be descriptive about it and to say what is expected and what we are testing. In this case we explicitly said: should return female when the name is from a female.


**Other thing to care about is the structure. A convention widely used is the AAA: Arrange, Act and Assert.**
- **Arrange**: you need to organize the data needed to execute that piece of code (input);
- **Act**: here you will execute the code being tested (exercise the behaviour);
- **Assert**: after executing the code, you will check if the result (output) is the same as you were expecting.

# If name equals main
## What does the if __ name__ == “__ main__”: do?
Before executing code, Python interpreter reads source file and define few special variables/global variables. 
If the python interpreter is running that module (the source file) as the main program, it sets the special __ name__ variable to have a value “__ main__”. If this file is being imported from another module, __ name__ will be set to the module’s name. Module’s name is available as value to __ name__ global variable. 

A module is a file containing Python definitions and statements. The file name is the module name with the suffix .py appended. 

Advantages : 

1. Every Python module has it’s __ name__ defined and if this is ‘__ main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.
1. If you import this script as a module in another script, the __ name__ is set to the name of the script/module.
1. Python files can act as either reusable modules, or as standalone programs.
if __ name__ == “main”: is used to execute some code only if the file was run directly, and not imported.

# Recursion
The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. Using recursive algorithm, certain problems can be solved quite easily. 

## A Mathematical Interpretation
Let us consider a problem that a programmer have to determine the sum of first n natural numbers, there are several ways of doing that but the simplest approach is simply add the numbers starting from 1 to n. So the function simply looks like,



    approach(1) – Simply adding one by one
    
    f(n) = 1 + 2 + 3 +……..+ n

but there is another mathematical approach of representing this,

    approach(2) – Recursive adding 

    f(n) = 1                  n=1

    f(n) = n + f(n-1)    n>1

There is a simple difference between the approach (1) and approach(2) and that is in approach(2) the function “ f( ) ” itself is being called inside the function, so this phenomenon is named as recursion and the function containing recursion is called recursive function, at the end this is a great tool in the hand of the programmers to code some problems in a lot easier and efficient way..


**How a particular problem is solved using recursion?**
The idea is to represent a problem in terms of one or more smaller problems, and add one or more base conditions that stop the recursion. For example, we compute factorial n if we know factorial of (n-1). The base case for factorial would be n = 0. We return 1 when n = 0. 


**Why Stack Overflow error occurs in recursion?**
If the base case is not reached or not defined, then the stack overflow problem may arise. Let us take an example to understand this.


**How memory is allocated to different function calls in recursion?** 
When any function is called from main(), the memory is allocated to it on the stack. A recursive function calls itself, the memory for a called function is allocated on top of memory allocated to calling function and different copy of local variables is created for each function call. When the base case is reached, the function returns its value to the function by whom it is called and memory is de-allocated and the process continues.
Let us take the example how recursion works by taking a simple function. 


**What are the disadvantages of recursive programming over iterative programming?** 
Note that both recursive and iterative programs have the same problem-solving powers, i.e., every recursive program can be written iteratively and vice versa is also true. The recursive program has greater space requirements than iterative program as all functions will remain in the stack until the base case is reached. It also has greater time requirements because of function calls and returns overhead.