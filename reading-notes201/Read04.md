# HTML Links, JS Functions, and Intro to CSS Layout

## links
Links are the defining feature of the web
because they allow you to move from
one web page to another — enabling the
very idea of browsing or surfing.

### Writing Links
Links are created using the < a> element. Users can click on anything
between the opening < a> tag and the closing < /a> tag. You specify
which page you want to link to using the href attribute.  

Links are created using the < a>
element which has an attribute
called href. The value of the
href attribute is the page that
you want people to go to when
they click on the link.

### Directory Structure

On larger websites it's a good idea to organize your code by placing the
pages for each different section of the site into a new folder. Folders on a
website are sometimes referred to as directories.  
- Structure:  
The diagram on the right shows
the directory structure for a
fictional entertainment listings
website called ExampleArts.
- Rela tionships:  
The relationship between
files and folders on a website
is described using the same
terminology as a family tree.
- Homepa ges:  
The main homepage of a site
written in HTML (and the
homepages of each section in a
child folder) is called index.html.

### Relative UR Ls
Relative URLs can be used when linking to pages within your own
website. They provide a shorthand way of telling the browser where to
find your files.
- Email Links

 *mailto:*  
 email-links.html HTML
To create a link that starts up
the user's email program and
addresses an email to a specified
email address, you use the < a>
element. However, this time the
value of the href attribute starts
with mailto: and is followed by
the email address you want the
email to be sent to.

- Op ening Links in
a New Window  

*target*  
If you want a link to open in a
new window, you can use the
target attribute on the opening
< a> tag. The value of this
attribute should be _blank.

## layout
In this chapter we are going to look at
how to control where each element sits
on a page and how to create attractive
page layouts.

### Key Concepts in Positioning El ements

- *Building Blocks*  
CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.
- *Containing Elements*  
If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.
### Controlling the Position of El ements

CSS has the following positioning schemes that allow you to control
the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.
- *Normal flow*  
Every block-level element
appears on a new line, causing
each item to appear lower down
the page than the previous one.
- *Relative Positioning*  
This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
 - *Ab olute positioning*  
This positions the element
in relation to its containing
element. It is taken out of
normal flow,
- *Fixed Positioning*  
This is a form of absolute
positioning that positions
the element in relation to the
browser window, as opposed
to the containing element.
- *Fixed Positioning*  
This is a form of absolute
positioning that positions
the element in relation to the
browser window, as opposed
to the containing element.

## Screen Sizes
Different visitors to your site will have different sized screens that show
different amounts of information, so your design needs to be able to
work on a range of different sized screens.
 ## Screen Resolution
Resolution refers to the number of dots a screen shows per inch. Some
devices have a higher resolution than desktop computers and most
operating systems allow users to adjust the resolution of their screens.
## Page Sizes
Because screen sizes and display resolutions vary so much, web
designers often try to create pages of around 960-1000 pixels wide
(since most users will be able to see designs this wide on their screens).
## Fixed Width Layouts
Fixed width layout
designs do not
change size as the
user increases
or decreases
the size of their
browser window.
Measurements tend
to be given in pixels.
## Liquid Layouts
Liquid layout designs
stretch and contract
as the user increases
or decreases the
size of their browser
window. They tend to
use percentages.

## CSS Frameworks
CSS frameworks aim to make your life easier by providing the code for
common tasks, such as creating layout grids, styling forms, creating
printer-friendly versions of pages and so on. You can include the CSS
framework code in your projects rather than writing the CSS from scratch.
- *ADVANTAGES*
1. They save you from
repeatedly writing code for
the same tasks.
2.  They will have been tested
across different browser
versions (which helps avoid
browser bugs).
- *ADVANTAGES*
1. They save you from
repeatedly writing code for
the same tasks.
2. They will have been tested
across different browser
versions (which helps avoid
browser bugs).

## Using the 960.GS Grid
Below you can see a sample layout of a page just like the fixed width
page example. On the next page, we will recreate this using the 960.gs
stylesheet. Instead of writing our own CSS to control layout, we will need
to add classes to the HTML indicating how wide each section should be.
## A Grid-Based Layout Using 960.GS
Let's take a look at an HTML
page and how it has been
marked up to use the 960.gs grid
system.
You can see that we include
the CSS for the grid using the
< link> element inside the
< head> of the page.

## Functions, Methods, and Objects
Browsers require very detailed instructions about what
we want them to do. Therefore, complex scripts can run
to hundreds (even thousands) of lines. Programmers use
functions, methods, and objects to organize their code.
This chapter is divided into three sections that introduce:
- FUNCTIONS & METHODS 
- OBJECTS
- BUILT-IN OBJECTS
### WHAT IS A FUNCTION?
Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of st atements).

## 6 Reasons for Pair Programming

### How does pair programming work
Pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard.

### Why pair program?
1. Greater efficiency   
It is a common misconception that pair programming takes a lot longer and is less efficient.

2. Engaged collaboration  
When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone.
3. Learning from fellow students  
Everyone has a different approach to problem solving; working with a teammate can expose developers to techniques they otherwise would not have thought of.
4. Social skills  
Pair programming is great for improving social skills. When working with someone who has a different coding style, communication is key. 
5. Job interview readiness  
A common step in many interview processes involves pair programming between a current employee and an applicant, either in person or through a shared screen.
6. Work environment readiness  
Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product.









