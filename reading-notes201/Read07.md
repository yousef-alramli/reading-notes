# Object-Oriented Programming, HTML Tables

## Domain Modeling
Domain modeling: is the process of creating a conceptual model in code for a specific problem

###  constructor and initialize properties
 constructor and initialize properties
 
 ### Generate random numbers

 To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a Math.random() function for just this sort of occasion.

 ### Calculate daily Likes
Popularity of a video is measured in Likes. And the formula for calculating Likes is the number of viewers times the percentage of viewers who'll Like a video. In other words, viewers times percentage.

## Tables

There are several types of information
that need to be displayed in a grid or
table. For example: sports results, stock
reports, train timetables.  

When representing information in a table, you need to think
in terms of a grid made up of rows and columns (a bit like a
spreadsheet). In this chapter you will learn how to:
- Use the four key elements for creating tables
-  Represent complex data using tables
- Add captions to tables

A **table** represents information in a grid format.
Examples of tables include financial reports, TV
schedules, and sports results.

### Basic Table Structure
< table>  
The < table> element is used
to create a table. The contents
of the table are written out row
by row.
< tr>  
You indicate the start of each
row using the opening <tr> tag.
(The tr stands for table row.)
It is followed by one or more
< td>   
elements (one for each cell
in that row).
At the end of the row you use a
closing < /tr> tag.
< td>  

Each cell of a table is
represented using a < td>
element. (The td stands for
table data.)
At the end of each cell you use a
closing < /td> tag.

### Old Code: Width & Spacing
There are some outdated
attributes which you should not
use on new websites. You may,
however, come across some
of them when looking at older
code, so I will mention them
here. All of these attributes have
been replaced by the use of CSS.

### Old Code: Border & Background
The border attribute was used
on both the < table> and < td>
elements to indicate the width of
the border in pixels.

## Functions, Methods, and Objects

### CREATING OBJECTS USING CONSTRUCTOR SYNTAX
to use the method,
you can use the object name
followed by the method name

### ADDING AND REMOVING PROPERTIES

Once you have created an object
(using literal or constructor
notation), you can add new
properties to it.  
You do this using the dot
notation that you saw for adding
properties to objects on pl03.

### RECAP: WAYS TO CREATE OBJECTS

1. CREATE THE OBJECT, THEN ADD PROPERTIES & METHODS
    - LITERAL NOTATION
    - OBJECT CONSTRUCTOR NOTATION

2. CREATING AN OBJECT WITH PROPERTIES & METHODS
    - LITERAL NOTATION: 
A colon separates the key/value pairs.
There is a comma between each key/value pair

    - OBJECT CONSTRUCTOR NOTATION: 
The function can be used to create multiple objects.
The this keyword is used instead of the object name.

### WHAT ARE BUILT-IN OBJECTS?
Browsers come with a set of built-in objects that represent things like the
browser window and the current web page shown in that window. These
built-in objects act like a toolkit for creating interactive web pages.  


The first thing you need to do is get to know what tools are available.
You can imagine that your new toolkit has three compartments:

1. BROWSER OBJECT
MODEL
The Browser Object Model contains
objects that represent the current
browser window or tab. It contains
objects that model things like
browser history and the
2. DOCUMENT OBJECT
MODEL
The Document Object Model uses
objects to create a representation of
the current page. It creates a new
object for each element (and each
individual section of text)
within the page.
3. GLOBAL JAVASCRIPT
OBJECTS
The global JavaScript objects
represent things that the JavaScript
language needs to create a model
of. For example, there is an
object that deals only with
dates and times.

### USING THE BROWSER OBJECT MODEL

Here, data about the browser is
col lected from the window object
and its children, stored in the msg
variable, and shown in the page.
The+= operator adds data onto
the end of the msg variable.  

1. Two of the window object's
properties, i nnerWi dth and
i nnerHei ght, show width and
height of the browser window.
JAVASCRIPT

2. Child objects are stored as
properties of t heir parent object.
So dot notation is used to access
them, just like you would access
any other property of that object.
In turn, to access the properties
of the child object, another dot is
used between the chi ld object's
name and its properties.

3. The element whose id
attribute has a value of info is
selected, and the message that
has been built up to this point is
written into the page.
See p228 for notes on using
i nnerHTML because it can be
a security risk if it is not used
correctly.

### WORKING WITH STRINGS
This example demonstrates the
1 ength property and many of the
string object's methods shown
on the previous page.
1. This example starts by storing
the phrase "Home sweet home "
in a variable ca lled saying.
JAVASCRIPT

2. The next line tells you how
many characters are in the string
using the 1 ength property of the
String object and stores the
result in a variable called msg.

3. This is followed by examples
showing several of the Stri ng
object's methods.  
The name of the variable
(saying) is followed by a dot,
then the property or method that
is being demonstrated (in the
same way that the other objects
in this chapter used the dot
notation to indicate a property or
method of an object).




