# Dunder Methods
What Are Dunder Methods?
In Python, special methods are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores, for example __ init__ or __ str__.

As it quickly became tiresome to say under-under-method-under-under Pythonistas adopted the term “dunder methods”, a short form of “double under.”

## Special Methods and the Python Data Model
This elegant design is known as the Python data model and lets developers tap into rich language features like sequences, iteration, operator overloading, attribute access, etc.

You can see Python’s data model as a powerful API you can interface with by implementing one or more dunder methods. If you want to write more Pythonic code, knowing how and when to use dunder methods is an important step.

## Enriching a Simple Account Class
Throughout this article I will enrich a simple Python class with various dunder methods to unlock the following language features:

- Initialization of new objects
- Object representation
- Enable iteration
- Operator overloading (comparison)
- Operator overloading (addition)
- Method invocation
- Context manager support (with statement)

# Iterators
## Python Iterators That Iterate Forever
We’ll begin by writing a class that demonstrates the bare-bones iterator protocol in Python. The example I’m using here might look different from the examples you’ve seen in other iterator tutorials, but bear with me. I think doing it this way gives you a more applicable understanding of how iterators work in Python.
## A Simpler Iterator Class
Up until now our iterator example consisted of two separate classes, Repeater and RepeaterIterator. They corresponded directly to the two phases used by Python’s iterator protocol:

First setting up and retrieving the iterator object with an iter() call, and then repeatedly fetching values from it via next().

Many times both of these responsibilities can be shouldered by a single class. Doing this allows you to reduce the amount of code necessary to write a class-based iterator.

# Generators
## Python Generators 101 – The Basics
Let’s start by looking again at the Repeater example that I previously used to introduce the idea of iterators. It implemented a class-based iterator cycling through an infinite sequence of values.
## Python Generators That Stop Generating
In this tutorial we started out by writing an infinite generator once again. By now you’re probably wondering how to write a generator that stops producing values after a while, instead of going on and on forever.

Remember, in our class-based iterator we were able to signal the end of iteration by manually raising a StopIteration exception. Because generators are fully compatible with class-based iterators, that’s still what happens behind the scenes.



