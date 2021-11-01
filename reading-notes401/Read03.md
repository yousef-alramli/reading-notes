# Reading and Writing Files in Python
## What Is a File?
A file is some information or data which stays in the computer storage devices. ... Python gives you easy ways to manipulate these files.

**Files on most modern file systems are composed of three main parts:**

1. Header: metadata about the contents of the file (file name, size, type, and so on)
1. Data: contents of the file as written by the creator or editor
1. End of file (EOF): special character that indicates the end of the file

### File Paths
An absolute file path describes how to access a given file or directory, starting from the root of the file system.
***we can break it up to three main parts:***
1. **Folder Path**: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
1. **File Name**: the actual name of the file
1. **Extension**: the end of the file path pre-pended with a period (.) used to indicate the file type

**example on file pathes as a tree:**  
    
    /
    |
    ├── path/   
    |   │  
    │   ├── to/  
    │   │   └── cats.gif  
    │   │  
    │   └── dog_breeds.txt  
    |  
    └── animals.csv

## Line Endings
The line edging character in Python is \n . It is used to indicate the end of a line of text.

This can make iterating over each line problematic, and you may need to account for situations like this.

## Character Encodings
A character encoding is one specific way of interpreting bytes: It's a look-up table that says, for example, that a byte with the value 97 stands for 'a'.

## Opening and Closing a File in Python
**Opening a file in python:**
There are two types of files that can be handled in Python, normal text files and binary files. Opening a file refers to getting the file ready either for reading or for writing. This can be done using the open() function. This function returns a file object and takes two arguments, one that accepts the file name and another that accepts the mode(Access Mode).
Note: The file should exist in the same directory as the Python script, otherwise, full address of the file should be written.

**Closing a file in Python:**
Python automatically closes a file if the reference object of the file is allocated to another file, it is a standard practice to close an opened file as a closed file reduces the risk of being unwarrantedly modified or read.
Python has a close() method to close a file. The close() method can be called more than once and if any operation is performed on a closed file it raises a ValueError. 
The below code shows a simple use of close() method to close an opened file.

# Python Exceptions
An exception is an event, which occurs during the execution of a program that disrupts the normal flow of the program's instructions. In general, when a Python script encounters a situation that it cannot cope with, it raises an exception. An exception is a Python object that represents an error.

## Exceptions versus Syntax Errors
**Syntax errors** are mistakes in the source code, such as spelling and punctuation errors, incorrect labels, and so on

**Exceptions:**

Even if a statement or expression is syntactically correct, it may cause an error when an attempt is made to execute it.

## Raising an Exception
Raising an exception is a technique for interrupting the normal flow of execution in a program, signaling that some exceptional circumstance has arisen, and returning directly to an enclosing part of the program that was designated to react to that circumstance.

## The try and except Block: Handling Exceptions ,else clause and finally
The **try** block lets you test a block of code for errors.

The **except** block lets you handle the error.

***Exception handling with try, exceptand else:***

- **Try**: This block will test the excepted error to occur
- **Except**:  Here you can handle the error
- **Else**: If there is no exception then this block will be executed
- **Finally**: Finally block always gets executed either exception is generated or not
Syntax: