# HTML Lists, Control Flow with JS, and the CSS Box Model
## Lists

There are lots of occasions when we
need to use lists. HTML provides us with
three different types:
-  Ordered lists are lists where each item in the list is
numbered. For example, the list might be a set of steps for
a recipe that must be performed in order, or a legal contract
where each point needs to be identified by a section
number.
-  Unordered lists are lists that begin with a bullet point
(rather than characters that indicate order).
- Definition lists are made up of a set of terms along with the
definitions for each of those terms.


### Ordered Lists
- The ordered list is created with
the < ol> element.
- Each item in the list is placed
between an opening < li> tag
and a closing < li> tag. (The li
stands for list item.)

### unordered Lists
- The unordered list is created
with the < ul> element.
- Each item in the list is placed
between an opening < li> tag
and a closing < /li> tag. (The li
stands for list item.)

### Definition Lists
- The definition list is created with
the < dl> element and usually
consists of a series of terms and
their definitions.
- < dt> This is used to contain the term
being defined (the definition
term).
- < dd> This is used to contain the
definition.


### nested LISTS 
You can put a second list inside
an < li> element to create a sublist
or nested list.

## Boxes

You can set several properties that affect the appearance of
these boxes. In this chapter you will see how to:
- Control the dimensions of your boxes
- Create borders around boxes
- Set margins and padding for boxes
- Show and hide boxes


### box Dimensions
By default a box is sized just big
enough to hold its contents. To
set your own dimensions for a
box you can use the height and
width properties.  

The most popular ways to
specify the size of a box are
to use pixels, percentages, or
ems. Traditionally, pixels have
been the most popular method
because they allow designers to
accurately control their size.

#### Limiting Width

Some page designs expand and
shrink to fit the size of the user's
screen. In such designs, the
min-width property specifies
the smallest size a box can be
displayed at when the browser
window is narrow, and the
max-width property indicates
the maximum width a box can
stretch to when the browser
window is wide.

#### Limting Height
In the same way that you might
want to limit the width of a box
on a page, you may also want
to limit the height of it. This is
achieved using the min-height
and max-height properties.

### Overflowing Content

- hidden: 
This property simply hides any
extra content that does not fit in
the box.
- scroll: 
This property adds a scrollbar to
the box so that users can scroll
to see the missing content.

### Border, Margin & Padding


1. Border
Every box has a border (even if
it is not visible or is specified to
be 0 pixels wide). The border
separates the edge of one box
from another.

2. Margin
Margins sit outside the edge
of the border. You can set the
width of a margin to create a
gap between the borders of two
adjacent boxes.  

3. Padding
Padding is the space between
the border of a box and any
content contained within it.
Adding padding can increase the
readability of its contents.

### Centering Content
If you want to center a box on
the page (or center it inside
the element that it sits in), you
can set the left-margin and
right-margin to auto.
In order to center a box on the
page, you need to set a width
for the box (otherwise it will take
up the full width of the page).
 
## Change Inline/Block

- inline
This causes a block-level
element to act like an inline
element.
- block
This causes an inline element to
act like a block-level element.
inline-block
This causes a block-level
element to flow like an inline
element, while retaining other
features of a block-level element.
- none
This hides an element from the
page. In this case, the element
acts as though it is not on the
page at all (although a user could
still see the content of the box if
they used the view source option
in their browser).

### Hiding boxes

The visibility property allows
you to hide boxes from users
but It leaves a space where the
element would have been.
This property can take two
values:
1. hidden: 
This hides the element.
2. visible: 
This shows the element.

## Basic JavaScript Instructions (Array)
An array is a special type of variable. It doesn't
just store one value; it stores a list of values.

### CREATING AN ARRAY
You create an array and give it
a name just like you would any
other variable (using the var
keyword followed by the name of
the array).

This technique for creating
an array is known as an array
literal. It is usually the preferred
method for creating an array.

### VALUES IN ARRAYS
Values in an array are accessed as if they are in
a numbered list. It is important to know that the
numbering of this list starts at zero (not one).
 
### ACCESSING & CHANGING VALUES IN AN ARRAY

The first lines of code on the left
create an array containing a list
of three colors. (The values can
be added on the same line or on
separate lines as shown here.)
Having created the array, the
third item on the list is changed
from 'custom' to 'beige'.

## Decisions and Loops

### IF ... ELSE STATEMENTS

if ... else statement allows you
to provide two sets of code:
1. one set if the condition
evaluates to true
2. another set if the condition is
false.

### SWITCH STATEMENTS
A switch statement starts with a
variable called the switch value.
Each case indicates a possible
value for this variable and the
code that should run if the
variable matches that value.

the purpose
of the switch statement is to
present the user with a different
message depending on which
level they are at. The message is
stored in a variable called msg.

### TYPE COERCION & WEAK TYPING
If you use a data type JavaScript did not expect,
it tries to make sense of the operation rather
than report an error.

### TRUTHY & FALSY VALUES
Due to type coercion, every value in JavaScript
can be treated as if it were true or false; and
this has some interesting side effects.

### CHECKING EQUALITY & EXISTENCE
Because the presence of an object or array can
be considered truthy, it is often used to check
for the existence of an element within a page.

### SHORT CIRCUIT VALUES
Logical operators are processed left to right.
They short-circuit (stop) as soon as they have a
result - but they return the value that stopped
the processing (not necessarily true or false).


### Loops
 Here are three points to consider when you
are working with loops:  

- KEYWORDS: 
You will commonly see these
two keywords used with loops(break & continue)

- LOOPS & ARRAYS: 
Loops are very helpful when
dealing with arrays if you want to
run the same code for each item
in the array.
- PERFORMANCE ISSUES
It is important to remember
that when a browser comes
across JavaScript, it will stop
doing anything else until it has
processed that script.

####  FOR LOOPS
A for loop is often used to loop
through the items in an array.
#### WHILE LOOPS
Here is an example of awhile
loop. It writes out the 5 times
table. Each time the loop is run,
another calculation is written
into the variable called msg.
#### DO WHILE LOOPS
The key difference between
a whi 1 e loop and a do whi 1 e
loop is that the statements in
the code block come before the
condition. This means that those
statements are run once whether
or not the condition is met.


