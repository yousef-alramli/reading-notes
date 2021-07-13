# Forms and JS Events

## Forms
Traditionally, the term 'form' has referred
to a printed document that contains
spaces for you to fill in information.

The best known form on the web is probably
the search box that sits right in the middle of
Google's homepage.

### Form Controls
1. ADDING TEXT:
    - Text input (single-line): 
Used for a single line of text such
as email addresses and names.
    - Password input: 
Like a single line text box but it
masks the characters entere
    - Text area (multi-line): 
For longer areas of text, such as
messages and comments.
2. Ma king Choices:
    - Radio buttons
For use when a user must select
one of a number of options.
    - Checkboxes: 
When a user can select and
unselect one or more options.
    -  Drop-down boxes: 
When a user must pick one of a
number of options from a list.
3. Submitting Forms:
    - Submit buttons: 
To submit data from your form
to another web page.
    - Image buttons
Similar to submit buttons but
they allow you to use an image.

4. Uploadi ng Files:
   - File upload
Allows users to upload files
(e.g. images) to a website

### How Forms Work


A user fills in a form and then presses a button
to submit the information to the server.

A form may have several form controls, each
gathering different information. The server
needs to know which piece of inputted data
corresponds with which form element.

## Lists, Tables and Forms

There are several CSS properties that
were created to work with specific types
of HTML elements, such as lists, tables,
and forms.

### Articl Point Styles
The list-style-type property
allows you to control the shape
or style of a bullet point (also
known as a marker).
It can be used on rules that
apply to the < ol>, < ul>, and < li>
elements.

### Images for bullets 
You can specify an image to act
as a bullet point using the
list-style-image property.

### list Shorthand
As with several of the other CSS
properties, there is a property
that acts as a shorthand for list
styles. It is called list-style,
and it allows you to express
the markers' style, image and
position properties in any order.

### table Properties

You have already met several
properties that are commonly
used with tables. Here we will
put them together in a single
example using the following:
width to set the width of the
table
padding to set the space
between the border of each table
cell and its content
text-transform to convert the
content of the table headers to
uppercase
letter-spacing, font-size
to add additional styling to the
content of the table headers
border-top, border-bottom
to set borders above and below
the table headers
text-align to align the writing
to the left of some table cells and
to the right of the others
background-color to change
the background color of the
alternating table rows
:hover to highlight a table row
when a user's mouse goes over it.

### Styling Forms
CSS is commonly used to
control the appearance of form
elements. This is both to make
them more attractive and to
make them more consistent
across different browsers
It is most common to style:
- Text inputs and text areas
- Submit buttons
- Labels on forms, to get the
form controls to align nicely

### cursor Styles
The cursor property allows
you to control the type of mouse
cursor that should be displayed
to users.

For example, on a form you
might set the cursor to be a hand
when the user hovers over it.

## Events
When you browse the web, your browser registers different
types of events. It's the browser's way of saying, "Hey, this
just happened." Your script can then respond to these events.

### DIFFERENT EVENT TYPES
Here is a selection of the events that occur in the browser while you are
browsing the web. Any of these events can be used to trigger a function
in your JavaScript code.

### HOW EVENTS TRIGGER JAVASCRIPT CODE

When the user interacts with the HTML on a web page, there are three
steps involved in getting it to trigger some JavaScript code.
Together these steps are known as event handling.
1. Select t he element
node(s) you want the
script to respond to.
2. Indicate which event on
the selected node(s) will
trigger the response.
3. State the code you want
to run when the event
occurs.

### USING EVENT LISTENERS
1. If you use a named function
when the event fi res on your
chosen DOM node, write that
function first. (You could also
use an anonymous function.)
2. The DOM element node(s) is
stored in a variable. Here the text
input (whose id attribute has a
value of username) is placed into
a variable called el Username.







