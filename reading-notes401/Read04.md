# Classes and Objects

**objects** are simply a collection of data (variables) and methods (functions) that act on those data. Similarly, a class is a blueprint for that object.

**class** is like an outline for creating a new object. An object is anything that you wish to manipulate or change while working through the code. Every time a class object is instantiated, which is when we declare a variable, a new object is initiated from scratch.

## Accessing Object Variables
The variables that are defined inside the methods can be accessed within that method only by simply using the variable name. Example – var_name. If you want to use that variable outside the method or class, you have to declared that variable as a global.

## Accessing Object Functions
To access a function inside of an object you use notation similar to accessing a variable.

# Thinking Recursively
**Recursive functions** are functions that calls itself. It is always made up of 2 portions, the base case and the recursive case. The base case is the condition to stop the recursion. The recursive case is the part where the function calls on itself.

### example on recursive finction :

    def factorial(x):

        if x == 1:
            return 1
        else:
            return (x * factorial(x-1))

input: 3
expected output: 6

## Maintaining State

When dealing with recursive functions, keep in mind that each recursive call has its own execution context, so to maintain state during recursion you have to either:

- Thread the state through each recursive call so that the current state is part of the current call’s execution context
- Keep the state in global scope

## Recursive Data Structures in Python
**recursive data structure** is a data structure that is partially composed of smaller or simpler instances of the same data structure. For example, linked lists and binary trees can be viewed as recursive data structures.

# Pytest Fixtures and Coverage

## fixtures
**Fixtures** define the steps and data that constitute the arrange phase of a test. 

In pytest, they are functions you define that serve this purpose. They can also be used to define a test's act phase; this is a powerful technique for designing more complex tests.
<br>
<br>
<br>
Improvements over xUnit-style setup/teardown functions
pytest fixtures offer dramatic improvements over the classic xUnit style of setup/teardown functions:

- fixtures have explicit names and are activated by declaring their use from test functions, modules, classes or whole projects.

- fixtures are implemented in a modular manner, as each fixture name triggers a fixture function which can itself use other fixtures.

- fixture management scales from simple unit to complex functional testing, allowing to parametrize fixtures and tests according to configuration and component options, or to re-use fixtures across function, class, module or whole test session scopes.

- teardown logic can be easily, and safely managed, no matter how many fixtures are used, without the need to carefully handle errors by hand or micromanage the order that cleanup steps are added.

## Fixture errors
pytest does its best to put all the fixtures for a given test in a linear order so that it can see which fixture happens first, second, third, and so on. If an earlier fixture has a problem, though, and raises an exception, pytest will stop executing fixtures for that test and mark the test as having an error.