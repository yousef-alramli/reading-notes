# What is functional programming?
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia

![](https://www.leadingagile.com/wp-content/uploads/2018/02/When-functional-programming-isnt.jpg)

Pure functions
Reading Files
If our function reads external files, it’s not a pure function — the file’s contents can change.


    const charactersCounter = (text) = >        Character count: ${text.length};

    function analyzeFile(filename) {
     let fileContent = open(filename);
    return charactersCounter(fileContent);
    }

**Random number generation**

    function yearEndEvaluation() {
    if (Math.random() > 0.5) {
    return "You get a raise!";
    } else {
    return "Better luck next year!";
    }
    }
Pure functions benefits The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:

Given a parameter A → expect the function to return value B
Given a parameter C → expect the function to return value D
A simple example would be a function to receive a collection of numbers and expect it to increment each element of this collection.

    let list = [1, 2, 3, 4, 5];

    const incrementNumbers = (list) => list.map(number => number + 1);

# Node JS Tutorial for Beginners #6 - Modules and require()

- What is a module?

a software component or part of a program that contains one or more routines. ... Modules make a programmer's job easy

- What does the word ‘require’ do?

 is intended to add separate pieces of code (“modules”) to the current scope, a feature 

- How do we bring another module into the file the we are working in?

By using import name and the path of the module

- What do we have to do to make a module available?

The first thing you do to get access to module features is export them. This is done using the export statement.