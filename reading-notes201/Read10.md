# Debugging
JavaScript can be hard to learn and everyone makes
mistakes when writing it. This chapter will help you learn
how to find the errors in your code. It will also teach you how
to write scripts that deal with potential errors gracefully.

## ORDER OF EXECUTION
To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run:

1. The greeting variable gets its value from the
greetUser() function.
2. greetUser() creates the message by combining
the string 'He 11 o ' with the result of getName ().
3. getName () returns the name to greetUser() .
4. greetUser() now knows the name, and combines
it with the string. It then returns the message to the
statement that ca lled it in step 1.
5. The va lue of the greeting is stored in memory.
6. This greeting variable is written to an alert box.
## EXECUT.ION CONTEXTS
1. EXECUTION CONTEXT
Every statement in a script lives in one of three
execution contexts:
- GLOBAL CONTEXT
Code that is in the script, but not in a function.
There is only one global context in any page.
- FUNCTION CONTEXT
Code that is being run within a function.
Each function has its own function context.
-  EVAL CONTEXT (NOT SHOWN)
Text is executed like code in an internal function
called eva l {) (which is not covered in this book).
2. VARIABLE SCOPE:

The first two execution contexts correspond with the
notion of scope (which you met on p98):
- GLOBAL SCOPE  
If a variable is declared outside a function, it can
be used anywhere because it has global scope.
If you do not use the var keyword when creating
a variable, it is placed in global scope.
- FUNCTION-LEVEL SCOPE  
When a variable is declared within a function,
it can only be used within that function. This is
because it has function-level scope.
## UNDERSTANDING SCOPE
In the interpreter, each execution context has its own va ri ables object.
It holds the variables, functions, and parameters available within it.
Each execution context can also access its parent's variables object.
## UNDERSTANDING ERRORS
If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handling code.
## HOW TO DEAL WITH ERRORS
Now that you know what an error is and how the browser treats them,
there are two things you can do with the errors.
1. DEBUG THE SCRIPT TO FIX ERRORS:  
If you come across an error while writing a script
(or when someone reports a bug), you will need to
debug the code, track down the source of the error,
and fix it.
You will find that the developer tools available in
every major modern browser will help you with
this task. In this chapter, you will learn about the
developer tools in Chrome and Firefox. (The tools in
Chrome are identical to those in Opera.)
IE and Safari also have their own tools (but there is
not space to cover them all).
2. HANDLE ERRORS GRACEFULLY:  
You can handle errors gracefully using try, catch,
throw, and f i na 1 ly statement s.
Sometimes, an error may occur in the script for a
reason beyond your control. For example, you might
request data from a third party, and their server
may not respond. In such cases, it is particularly
important to write error-handling code.
In the latter part of the chapter, you will learn how to
gracefully check whether something will work, and
offer an alternative option if it fails.
## A DEBUGGING WORKFLOW
Debugging is about deduction: eliminating potential causes of an error.
Here is a workflow for techniques you will meet over the next 20 pages.
Try to narrow down where the problem might be, then look for clues.

## BROWSER DEV TOOLS & JAVASCRIPT CONSOLE
The JavaScript console will tell you when there is a problem with a script,
where to look for the problem, and what kind of issue it seems to be.
These two pages show instructions for opening the
console in all of the main browsers (but the rest of
this chapter will focus on Chrome and Firefox).
* CHROME/ OPERA
![](https://www.steveworkman.com/static/img/opera-chrome.jpg)

On a PC, press the F12 key or:
1. Go to the options menu (or three line menu icon)
2. Select Toots or More tools.
3. Select JavaScript Console or Developer Tools
On a Mac press Alt + Cmd + J. Or:
4. Go to the View menu.
5. Select Developer.
6. Open the JavaScript Console or Developer Tools
option and select Console.
* INTERNET EXPLORER
![](https://www.computerhope.com/jargon/m/msedge-300.jpg)
Press the F12 key or:
1. Go to the settings menu in the top-right.
2. Select developer tools.

## BREAKPOINTS
You can pause the execution of a script on any
line using breakpoints. Then you can check the
va lues stored in variables at that point in time.
## STEPPING THROUGH CODE
When you have set breakpoints,
you will see that the debugger
lets you step through the code
line by line and see the values
or variables as your script
progresses.
When you are doing this, if
the debugger comes across a
function, it will move onto the
next line after the function.
(It does not move to where
the function is defined.) This
behavior is sometimes called
stepping over a function.
If you want to, it is possible
to tell the debugger to step
into a function to see what is
happening inside the function.
If you set multiple breakpoints, you can step
through them one-by-one to see where values
change and a problem might occur.

## CONDITIONAL BREAKPOINTS
You can indicate that a breakpoint should be
triggered only if a condition that you specify is
met. The condition can use existing variables.
8 ERROR HANDLING & DEBUGGING
CHROME
1. Right-click on a line number.
2. Select Add Conditional
Breakpoint...
3. Enter a condition into the
popup box.
4 . When you run the script, it
will only stop on this line if the
condition is true (e.g., if area is
less than 20).
FIREFOX
1. Right-click on a line of code.
2. Select Add conditional
breakpoint.
3. Enter a condition into the
popup box.
4. When you run the script, it
will stop on this line only if the
condition is true (e.g., if area is
less than 20).

## TRY, CATCH, FINALLY
This example displays JSON data
to the user. But, imagine that the
data is coming from a third party
and there have been occasional
problems with it that could
cause the page to fail.
This script checks if the JSON
can be parsed using a try block
before trying to di splay the
information to the users.
JAVASCRIPT
If the try statement throws an
error (because the data cannot
be parsed), the code in the catch
code block will be run, and the
error will not prevent the rest of
the script from being executed.
The catch statement creates
a message using the name and
message properties of the Error
object.
The error will be logged to the
console, and a friendly message
will be shown to the users of
the site. You cou ld also send
the error message to the server
using Ajax so that it could
be recorded. Either way, the
f i na 11 y statement adds a link
that allows users to refresh the
data they are seeing.

## DEBUGGING TIPS
Here are a selection of practical tips that you
can try to use when debugging your scripts.  
- ANOTHER BROWSER  
Some problems are browserspecific.
Try the code in another
browser to see which ones are
causing a problem.
- ADD NUMBERS  
Write numbers to the console
so you can see which the items
get logged. It shows how far your
code runs before errors stop it.
- STRIP IT BACK  
Remove parts of code, and strip
it down to the minimum you
need. You can do this either by
removing the code altogether, or
by just commenting it out using
multi-line comments:
/* Anything between these
characters is a cofllllent */
- EXPLAINING THE CODE  
Programmers often report
finding a solution to a problem
while explaining the code to
someone else.
- SEARCH  
Stack Overflow is a Q+A site for
programmers.
Or use a traditional search
engine such as Google, Bing, or
DuckDuckGo.  
- CODE PLAYGROUNDS
If you want to ask about
problematic code on a forum, in
addition to pasting the code into
a post, you could add it to a code
playground site (such as
JSBin.com, JSFiddle. com, or
Dabbl et. corn) and then post a
link to it from the forum.
(Other popular playgrounds
include CSSDeck. com and
Code Pen. com - but these sites
place more emphasis on show
and tell.)
- VALIDATION TOOLS
There are a number of on line
validation tools that can help you
try to find errors in your code:
    - JAVASCRIPT
http://www.jslint.com
http://www.jshint .com
     - JSON
http:// www.jsonlint.com
    - JQUERY
There is a jQuery debugger
plugin available for Chrome
which can be found in the
Chrome web store.







