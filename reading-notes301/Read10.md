# The JavaScript Call Stack

The JavaScript engine (which is found in a hosting environment like the browser), is a single-threaded interpreter comprising of a heap and a single call stack. The browser provides web APIs like the DOM, AJAX, and Timers.

![](https://miro.medium.com/max/638/1*CCHexfHNCNo-f8aw3rbRew.jpeg)

This article is aimed at explaining what the call stack is and why it is needed. An understanding of the call stack will give clarity to how “function hierarchy and execution order” works in the JavaScript engine.

The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

## Manage function invocation (call)
The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.

In summary
The key takeaways from the call stack are:

- It is single-threaded. Meaning it can only do one thing at a time.
- Code execution is synchronous.
- A function invocation creates a stack frame that occupies a temporary memory.
- It works as a LIFO — Last In, First Out data structure.
## JavaScript error messages && debugging
Most of your time as a developer is spent reading code followed by debugging that same code, most likely to be able to read it or solve an “unexpected feature” (which, joking aside, is more correctly known as a “bug”).

# JavaScript error messages && debugging
Most of your time as a developer is spent reading code followed by debugging that same code, most likely to be able to read it or solve an “unexpected feature” (which, joking aside, is more correctly known as a “bug”).

This is a sample of an error, the green is the overall error message, the light blue is to note if the error was properly handled, the brownish (dark yellow) is the type of error and the red is the call stack

## Types of error messages
- Reference errors

This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

- Syntax errors

I know it’s in the name of the errors, but like it says itself, this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

- Range errors

Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up. 

- Type errors

Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.
 ## Debugging

To debug your JS code, the easiest and maybe the most common way its to simply console.log() the variables you want to check or, by using chrome developer tools, open your page with your JS code (press cmd+o in macOS or Ctrl+o in Windows) and choose your file to debug, click the line you wanna debug and refresh your page again (F5).
If the line you selected was run you will be able to see what has happened before that point and you can try and evaluate the next lines to check if everything is outputting what you are expecting.
The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.
