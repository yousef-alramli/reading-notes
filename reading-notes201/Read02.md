# Basics of HTML, CSS & JS summary

## text summary 

When creating a web page, you add tags
(known as markup) to the contents of the
page. These tags provide extra meaning
and allow browsers to show users the
appropriate structure for the page.

### Headings

HTML has six "levels" of
headings:  

- <h 1> is used for main headings
- <h 2> is used for subheadings
If there are further sections
under the subheadings then the
- <h 3> element is used, and so
on...


### Paragraphs

To create a paragraph, surround
the words that make up the
paragraph with an opening < p>
tag and closing </ p> tag.  

By default, a browser will show
each paragraph on a new line
with some space between it and
any subsequent paragraphs.


### Bold & It alic
- By enclosing words in the tags
<b> and </b> we can make
characters appear bold.   


- By enclosing words in the tags
<i> and </i> we can make
characters appear italic.  


### Superscript & Subscript

- The <su p> element is used
to contain characters that
should be superscript such
as the suffixes of dates or
mathematical concepts like
raising a number to a power such
as 22.

- The <su b> element is used to
contain characters that should
be subscript. It is commonly
used with foot notes or chemical
formulas such as H20.


### Line Breaks & Horizontal Rules

- As you have already seen, the
browser will automatically show
each new paragraph or heading
on a new line. But if you wanted
to add a line break inside the
middle of a paragraph you can
use the line break tag <br / >.

- To create a break between
themes — such as a change of
topic in a book or a new scene
in a play — you can add a
horizontal rule between sections
using the <hr / > tag.

### Visual Editors

Visual editors often resemble
word processors. Although
each editor will differ slightly,
there are some features that
are common to most editors
that allow you to control the
presentation of text.

### Semantic Markup

There are some text elements that are not intended to affect the
structure of your web pages, but they do add extra information to the
pages — they are known as semantic markup.

### St rong & Emph asis
The use of the < st rong >
element indicates that its
content has strong importance.
For example, the words
contained in this element might
be said with strong emphasis.  


The < e m > element indicates
emphasis that subtly changes
the meaning of a sentence.

### Quotations

- The < q> element is used for
shorter quotes that sit within
a paragraph.
- The < blockquote> element is
used for longer quotes that take
up an entire paragraph.

### Citations & Definitions

- the
< cite> element can be used
to indicate where the citation is
from.

- The < dfn> element is used to
indicate the defining instance of
a new term.

### Auth or Details
 
 The < address> element has
quite a specific use: to contain
contact details for the author of
the page.

### Changes to Content

- The < ins> element can be used
to show content that has been
inserted into a document, while
the < del> element can show text
that has been deleted from it.
- The < s> element indicates
something that is no longer
accurate or relevant

## Introducing CSS
CSS allows you to create rules that specify how the content of
an element should appear. For example, you can specify that
the background of the page is cream, all paragraphs should
appear in gray using the Arial typeface, or that all level one
headings should be in a blue, italic, Times typeface.

- CSS allows you to create rules that control the
way that each individual box (and the contents
of that box) is presented.

- CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts: a selector and a declaration.

- CSS declarations sit inside curly brackets and each is made up of two
parts: a property and a value, separated by a colon. You can specify
several properties in one declaration, each separated by a semi-colon.

### Usi ng External CSS
- The < link> element can be used
in an HTML document to tell the
browser where to find the CSS
file used to style the page
- href
This specifies the path to the
CSS file (which is often placed in
a folder called css or styles).
- type
This attribute specifies the type
of document being linked to. The
value should be text/css.
- rel
This specifies the relationship
between the HTML page and
the file it is linked to. The value
should be stylesheet when
linking to a CSS file.
### Usi ng Internal CSS

You can also include CSS rules
within an HTML page by placing
them inside a < style> element, which usually sits inside the
< head> element of the page.
### CSS Selectors
There are many different types
of CSS selector that allow you to
target rules to specific elements
in an HTML document.


CSS selectors are case sensitive,
so they must match element
names and attribute values
exactly.

### How Css Rules Cascade

#### LAST RULE
If the two selectors are identical,
the latter of the two will take
precedence. Here you can see
the second i selector takes
precedence over the first.
#### SPECIFICITY
If one selector is more specific
than the others, the more
specific rule will take precedence
over more general ones. In this

#### IMPORTANT
You can add !important after
any property value to indicate
that it should be considered
more important than other rules
that apply to the same element.
 
### Why use External Style Sheets?
When building a website there are several advantages to placing your
CSS rules in a separate style sheet.


**CSS rules usually appear in a separate document,
although they may appear within an HTML page.**

## Basic JavaScript Instructions

### STATEMENTS

A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
Statements should end with a semicolon.

### COMMENTS
comments are to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read your code

### VARIABLEs
A script will have to temporarily
store the bits of information it
needs to do its job. It can store this
data in variables.


When you write JavaScript, you have to tell the
interpreter every individual step that you want it to
perform. This sometimes involves more detail than
you might expect.


#### A variable is a good name for this concept because the data stored.



in a variable can change (or vary)
each time a script runs.
No matter what the dimensions of any individual
wall are, you know that you can fin d its area by
multiplying the width of that wall by its height.
Similarly, scripts often need to achieve the same
goal even when they are run with different data, so
variables can be used to represent values in your
scripts that are likely to change. The result is said to
be calculated or computed using the data stored in
the variables.

### DATA TYPES

- NUMERIC DATA TYPE: 
The numeric data type handles
numbers.
- STRING DATA TYPE: 
The strings data type consists of
letters and other characters.
- BOOLEAN DATA TYPE
Boolean data types can have one
of two va lues: true or false.

#### USINGS Of VARIABLES

- USING A VARIABLE TO
STORE A NUMBER
- USING A VARIABLE TO
STORE A STRING
- USING QUOTES
INSIDE A STRING
- USING A VARIABLE TO
STORE A BOOLEAN
- SHORTHAND FOR
CREATING VARIABLES
-CHANGING THE VALUE
OF A VARIABLE

### RULES FOR NAMING VARIABLES

1. The name must begin with
a letter, dollar sign ($),or an
underscore (_). It must not start
with a number.

2.  The name can contain letters,
numbers, dollar sign ($), or an
underscore (_). Note that you
must not use a dash(-) or a
period (.) in a variable name.

3. You cannot use keywords or
reserved words. Keywords
are special words that tell the
interpreter to do something. For
example, var is a keyword used
to declare a variable. Reserved
words are ones that may be used
in a future version of JavaScript.
ONLINE EXTRA
View a full list of keywords and
reserved words in JavaScript.
4. All variables are case sensitive,
so score and Score would be
different variable names, but
it is bad practice to create two
variables that have the same
name using different cases.
5. Use a name that describes the
kind of information that the
variable stores. For example,
fi rstName might be used to
store a person's first name,
l astNarne for their last name,
and age for their age.
6. If your variable name is made
up of more than one word, use a
capital letter for the first letter of
every word after the first word.
For example, f i rstName rather
than fi rstnarne (this is referred
to as camel case).

### ARRAYS
An array is a special type of variable. It doesn't
just store one value; it stores a list of values.

You should consider using an
array whenever you are working
with a list or a set of values that
are related to each other.

#### CREATING AN ARRAY
You create an array and give it
a name just like you would any
other variable (using the var
keyword followed by the name of
the array).  

The values are assigned to the
array inside a pair of square
brackets, and each value is
separated by a comma. The
values in the array do not need
to be the same data type, so you
can store a string, a number and
a Boolean all in the same array.

#### VALUES IN ARRAYS
- NUMBERING ITEMS IN
AN ARRAY
Each item in an array is
automatically given a number
called an index. This can be used
to access specific items in the
array. Consider the following
array which holds three colors:
- ACCESSING ITEMS IN
AN ARRAY
To retrieve the third item on the
list, the array name is specified
along with the index number in
square brackets.
- NUMBER OF ITEMS IN
AN ARRAY
Each array has a property called
length, which holds the number
of items in the array.

### EXPRESSIONS

1. EXPRESSIONS THAT JUST ASSIGN A
VALUE TO A VARIABLE
2. EXPRESSIONS THAT USE TWO OR
MORE VALUES TO RETURN A
SINGLE VALUE.

### OPERATORS
Expressions rely on things called operators; they allow programmers to
create a single value from one or more values.


 **Types of operators:**
- ARITHMETIC OPERATORS
- STRING OPERATOR

## Decisions and Loops
Looking at a flowchart (for all but the most basic scripts),
the code can take more than one path, which means the
browser runs different code in different situations.

* EVALUATIONS
You can analyze values in
your scripts to determine
whether or note they
match expected results.

* DECISIONS
Using the results of
evaluations, you can
decide which path your
script should go down.
* LOOPS
There are also many
occasions where you will
want to perform the same
set of steps repeatedly.




