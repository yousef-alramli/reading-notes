# Python Scope & the LEGB Rule
the concept of scope is closely related to the concept of the namespace. As you've learned so far, a Python scope determines where in your program a name is visible. Python scopes are implemented as dictionaries that map names to objects. These dictionaries are commonly called namespaces.

### there's two general scopes:

1. Global scope: The names that you define in this scope are available to all your code.

1. Local scope: The names that you define in this scope are only available or visible to the code within the scope.

## Using the LEGB Rule for Python Scope

- **local (or function) scope** is the code block or body of any Python function or lambda expression. This Python scope contains the names that you define inside the function. These names will only be visible from the code of the function. It’s created at function call, not at function definition, so you’ll have as many different local scopes as function calls. This is true even if you call the same function multiple times, or recursively. Each call will result in a new local scope being created.

- **Enclosing (or nonlocal) scope** is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function. This scope contains the names that you define in the enclosing function. The names in the enclosing scope are visible from the code of the inner and enclosing functions.

- **Global (or module) scope** is the top-most scope in a Python program, script, or module. This Python scope contains all of the names that you define at the top level of a program or a module. Names in this Python scope are visible from everywhere in your code.

- **Built-in scope** is a special Python scope that’s created or loaded whenever you run a script or open an interactive session. This scope contains names such as keywords, functions, exceptions, and other attributes that are built into Python. Names in this Python scope are also available from everywhere in your code. It’s automatically loaded by Python when you run a program or script.

## The Global Scope
In computer programming, a global variable is a variable with global scope, meaning that it is visible (hence accessible) throughout the program, unless shadowed. The set of all global variables is known as the global environment or global state.

There’s only one global Python scope per program execution. This scope remains in existence until the program terminates and all its names are forgotten. Otherwise, the next time you were to run the program, the names would remember their values from the previous run.


Whenever you assign a value to a name in Python, one of two things can happen:

1. You create a new name
1. You update an existing name

  
**Global names can be updated or modified from any place in your global Python scope. Beyond that, the global statement can be used to modify global names from almost any place in your code, as you’ll see in The global Statement.**

Modifying global names is generally considered bad programming practice because it can lead to code that is:

* Difficult to debug: Almost any statement in the program can change the value of a global name.
* Hard to understand: You need to be aware of all the statements that access and modify global names.
* Impossible to reuse: The code is dependent on global names that are specific to a concrete program.

Good programming practice recommends using local names rather than global names. Here are some tips:

* Write self-contained functions that rely on local names rather than global ones.
* Try to use unique objects names, no matter what scope you’re in.
Avoid global name modifications throughout your programs.
* Avoid cross-module name modifications.
* Use global names as constants that don’t change during your program’s execution.

Following the LEGB rule, you’ll look up number in the following places:

- Inside inner_func(): This is the local scope, but number doesn’t exist there.
- Inside outer_func(): This is the enclosing scope, but number isn’t defined there either.
- In the module scope: This is the global scope, and you find number there, so you can print number to the screen.

### example on global:

    def myfunction():
    global x
    x = "hello"

    myfunction()

    print(x)

    output => hello


## The nonlocal Statement

The nonlocal keyword is used to work with variables inside nested functions, where the variable should not belong to the inner function. Use the keyword nonlocal to declare that the variable is not local.

The nonlocal statement consists of the nonlocal keyword followed by one or more names separated by commas. These names will refer to the same names in the enclosing Python scope. 

### example on nonlocal:

    def myfunc1():
      x = "John"
      def myfunc2():
        nonlocal x
        x = "hello"
      myfunc2()
      return x

    print(myfunc1())

    output => hello


# Big O Notation
Big-O notation is a metrics used to find algorithm complexity. Basically, Big-O notation signifies the relationship between the input to the algorithm and the steps required to execute the algorithm. It is denoted by a big "O" followed by opening and closing parenthesis.

# Rolling Dice Examples:

    from random import randint

    def roll_dice():
        print(f"Number is: {randint (1,6)}")

    roll_dice()
    
    output => Number is **number between 1 and 6**