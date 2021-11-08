# List Comprehensions in Python

**List comprehensions** are used for creating new lists from other iterables like tuples, strings, arrays, lists, etc. A list comprehension consists of brackets containing the expression, which is executed for each element along with the for loop to iterate over each element.

## Syntax
**the list comprehension syntax contains three parts:** 
1. an expression
2. one or more for loop
3. and optionally one or more if conditions.

## Notes about Lists Comprehensions
- List comprehension methods are an elegant way to create and manage lists. 
- In Python, list comprehensions are a more compact way of creating lists. 
- More flexible than for loops, list comprehension is usually faster than other methods.

## Create a List with range()
Example:  
digits = [x for x in range(10)]

In the python example above, we’re using the range() method to generate a list of numbers. Python iterates(or loops) through each item in that range, and saves a copy of the item in a new list called digits.

## Create a List Using Loops and List Comprehension in Python

Example:  
for x in range(10):
    # raise x to the power of 2
    squares.append(x**2)

## Lower/Upper case converter using Python

Making use of Python’s lower() and upper() methods, we’ll use list comprehension to achieve this common task.

Example:  
lower_case = [ letter.lower() for letter in ['A','B','C'] ]
upper_case = [ letter.upper() for letter in ['a','b','c'] ]

# Primer on Python Decorators

## Functions
 a **function** is a named section of a code that performs a specific task. This typically involves taking some input, manipulating the input and returning an output.

 ### First-Class Objects
 In Python, functions are first-class objects. This means that functions can be passed around and used as arguments, just like any other object (string, int, float, list, and so on).

### Inner Functions
**Inner functions**, also known as nested functions, are functions that you define inside other functions.

## Simple Decorators

A **decorator** is a design pattern in Python that allows a user to add new functionality to an existing object without modifying its structure. Decorators are usually called before the definition of a function you want to decorate

## Fancy Decorators
*Decorators* are one of the most helpful and powerful tools of Python. These are used to modify the behavior of the function. In Decorators, functions are passed as an argument into another function and then called inside the wrapper function.

