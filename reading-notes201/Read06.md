#  Problem Domain, Objects, and the DOM
## Understanding The Problem Domain Is The Hardest Part Of Programming
hardest things abou coing:
- Learning a new technology
- Naming things
- Testing your code
- Debugging
- Fixing bugs
- Making software maintainable
### Why problem domains are hard
The reason why puzzles like this one are so hard, is because you can’t really see what you are trying to build very clearly.  Normally when you put together a jigsaw puzzle you follow steps that might look something like this:
- Figure out what the major - components of the picture are
- Sort the pieces by color or component
- Put together all the border pieces
- Put together each component of the picture from the piles you created
The real world is a messy place.  Many of the problem domains we face as programmers are difficult to understand and look completely different depending on your viewpoint.

It is easy to fall into the trap of thinking you understand enough of the problem to get started coding it.

## Object Literals
### WHAT IS AN OBJECT?
Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names.
- IN AN OBJECT: VARIABLES BECOME
KNOWN AS PROPERTIES
If a variable is part of an object, it is called a
property. Properties te ll us about the object, such as
the name of a hotel or the number of rooms it has.
Each individual hotel might have a different name
and a different number of rooms.
- IN AN OBJECT: FUNCTIONS BECOME
KNOWN AS METHODS
If a function is part of an object, it is called a method.
Methods represent tasks that are associated with
the object. For example, you can check how many
rooms are available by subtracting the number of
booked rooms from the total number of rooms.
### CREATING· OBJECTS USING
LITERAL NOTATION

This example starts by creating
an object using litera l notation.
This object is called hotel which
represents a hotel called Quay
with 40 rooms (25 of which have
been booked).
Next, the content of the page
is updated with data from this
object. It shows the name of the
hotel by accessing the object's
name property and the number
of vacant rooms using the
checkAvail ability() method.
To access a property of this
object, the object name is
followed by a dot (the period
symbol) and the name of the
property that you want.
Similarly, to use the method,
you can use the object name
followed by the method name.
hotel .checkAvailability()
If the method needs parameters,
you can supply them in the
parentheses (just like you can
pass arguments to a funct ion).

(c3/ j s/obj ect-1itera1 . j s
var hotel = {
name: 'Quay',
rooms : 40,
booked: 25,
checkAvailability: function() {
return this.rooms - this.booked;
}
} ;
JAVASCRIPT
var elName = document .getElementByld('hotelName');
elName.textContent =hotel .name;
var elRooms = document.getElementByid{'rooms');
elRooms .textContent = hotel .checkAvailability();)


### CREATING MORE OBJECT LITERALS
The only things changing in the
code are the va lues of the hot e 1
object's properties:
- The name of the hotel
- How many rooms it has
- How many rooms are booked

## Document Object Model
The Document Object Model (DOM) specifies
how browsers should create a model of an HTML
page and how JavaScript can access and update the
contents of a web page while it is in the browser window.  

The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules.
It is implemented by all major browser makers, and covers two primary areas:

- MAKING A MODEL OF THE
HTML PAGE  

When the browser loads a web page, it
creates a model of the page in memory.
The DOM specifies the way in which the
browser should structure this model using
a DOM tree.
The DOM is called an object model
because the model (the DOM tree) is
made of objects.
Each object represents a different part of
the page loaded in the browser window.
s DOCUMENT OBJECT MODEL
- ACCESSING AND CHANGING
THE HTML PAGE  

The DOM also defines methods and
properties to access and update each
object in this model, which in turn updates
what the user sees in the browser.
You will hear people call the DOM an
Application Programming Interface (API).
User interfaces let humans interact with
programs; APls let programs (and scripts)
talk to each other. The DOM states what
your script can "ask the browser about the
current page, and how to tell the browser
to update what is being shown to the user.

### WORKING WITH THE DOM TREE
Accessing and updating the DOM tree involves two steps:
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes.


### ACCESSING ELEMENTS
DOM queries may return one element, or they may return a Nodelist,
which is a collection of nodes.
### SELECTING ELEMENTS USING ID ATTRIBUTES
get El ementByid () al lows you
to select a single element node
by specifying the value of its
id attribute.
### NODELISTS: DOM QUERIES THAT RETURN MORE THANONE ELEMENT
LIVE & STATIC NODELISTS  
There are times when you will want to work with
the same selection of elements several times, so
the Nodelist can be stored in a variable and re -used
(rather than collecting the same elements again).

### SELECTING ELEMENTS USING CLASS ATTRIBUTES
The get El ementsByCl ass Name()
method allows you to select
elements whose c 1 ass attribute
contains a specific value.  

The method has one parameter:  
the class name which is given
in quotes within the parentheses
after the method name.
Because several elements can
have the same value for their
cl ass attribute, this method
always returns a Nodelist.
### SELECTING ELEMENTS
BY TAG NAME
The get El ementsByTagName ()
method allows you to select
elements using their tag name.
JAVASCRIPT
The element name is specified
as a parameter, so it is placed
inside the parentheses and is
contained by quote marks.
Note that you do not include the
angled brackets that surround
the tag name in the HTML (just
the letters inside the brackets).
### SELECTING ELEMENTS
USING CSS SELECTORS
querySe 1 ector() returns
the first element node that
matches the CSS-style selector.
querySe 1ectorA11 () returns a
Nodelist of all of the matches.
### LOOPING THROUGH
A NODELIST
If you want to apply the same
code to numerous elements,
looping through a Nodelist is a
powerful technique.

### TRAVERSING THE DOM
- parentNode  
This property finds the element
node for the containing (or
parent) element in the HTML.
 previousSibling
- nextSibling  
These properties find the
previous or next sibling of a node
if there are siblings.
- firstChild
lastChild
These properties find the first or
last child of the current element.

### HOW TO GET/UPDATE
ELEMENT CONTENT
So far this chapter has focused on finding elements in the DOM tree.
The rest of this chapter shows how to access/update element content.
Your choice of techniques depends upon what the element contains.

### ACCESS & UPDATE A TEXT NODE WITH NODEVALUE
When you select a text node, you can retrieve or amend the content of it
using the node Va 1 ue property.

### ACCESS & UPDATE TEXT
WITH TEXTCONTENT
(& INN ERTEXT)
The textCon tent property allows you to
collect or update just the text that is in the
containing element (and its children).
### DOM MANIPULATION DOM manipulation offers another technique
to add new content to a page (rather than
i nnerHTML). It involves three steps:
1. CREATE THE ELEMENT  
2. GIVE IT CONTENT
3. ADD IT TO THE DOM

### ADDING AN ELEMENT TO
THE DOM TREE
createEl ement () creates an
element that can be added to the
DOM tree, in this case an empty
< li >element for the list.
### REMOVING ELEMENTS VIA DOM MANIPULATION
DOM manipulation can be used to remove
elements from the DOM tree.
1. STORE THE ELEMENT
TO BE REMOVED IN A
VARIABLE
You start by selecting the
element that is going to be
removed and store that element
node in a variable.
You can use any of the methods
you saw in the section on DOM
queries to select the element.
2. STORE THE PARENT OF
THAT ELEMENT IN A
VARIABLE
Next, you find the parent element
that contains the element you
want to remove and store that
element node in a variable.
The simplest way to get this
element is to use the parentNode
property of this element.

3. REMOVE THE ELEMENT
FROM ITS CONTA INING
ELEMENT
The removeChi ld() method is
used on the containing element
that you selected in step 2.
The removeChi ld() method
takes one parameter: the
reference to the element that
you no longer want.

### CROSS-SITE SCRIPTING
(XSS) ATTACKS
If you add HTML to a page using i nnerHTML (or several jQuery methods),
you need to be aware of Cross-Site Scripting Attacks or XSS; otherwise,
an attacker could gain access to your users' accounts.
### DEFENDING AGAINST
CROSS-SITE SCRIPTING
VALIDATE INPUT GOING TO THE SERVER
1. Only let visitors input the kind
of characters they need to when
supplying information. This is
known as validation. Do not
allow untrusted users to submit
HTML markup or JavaScript.
2. Double-check validation on
the server before displaying user
content/storing it in a database.
This is important because users
could bypass validation in the
browser by turning JavaScript off.
3. The database may safely
contain markup and script
from trusted sources (e.g., your
content management system).
This is because it does not try to
process the code; it just stores it.














