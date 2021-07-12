## layout
In this chapter we are going to look at
how to control where each element sits
on a page and how to create attractive
page layouts.

### Key Concepts in Positioning El ements

- *Building Blocks*  
CSS treats each HTML element as if it is in its
own box.
- *Containing Elements*  
If one block-level element sits inside another
block-level element then the outer box is
known as the containing or parent element.
### Controlling the Position of Elements

CSS has the following positioning schemes that allow you to control
the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.
- **Normal flow**  
Every block-level element
appears on a new line, causing
each item to appear lower down
the page than the previous one.
- **Relative Positioning**  
This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
 - **Absolute positioning**  
This positions the element
in relation to its containing
element. It is taken out of
normal flow,
- **Fixed Positioning**  
This is a form of absolute
positioning that positions
the element in relation to the
browser window, as opposed
to the containing element.
- **Fixed Positioning**  
This is a form of absolute
positioning that positions
the element in relation to the
browser window, as opposed
to the containing element.

### Screen Sizes
Different visitors to your site will have different sized screens that show
different amounts of information, so your design needs to be able to
work on a range of different sized screens.
 ### Screen Resolution
Resolution refers to the number of dots a screen shows per inch. Some
devices have a higher resolution than desktop computers and most
operating systems allow users to adjust the resolution of their screens.
### Page Sizes
Because screen sizes and display resolutions vary so much, web
designers often try to create pages of around 960-1000 pixels wide
(since most users will be able to see designs this wide on their screens).
### Fixed Width Layouts
Fixed width layout
designs do not
change size as the
user increases
or decreases
the size of their
browser window.
Measurements tend
to be given in pixels.
### Liquid Layouts
Liquid layout designs
stretch and contract
as the user increases
or decreases the
size of their browser
window. They tend to
use percentages.

### CSS Frameworks
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

### Using the 960.GS Grid
Below you can see a sample layout of a page just like the fixed width
page example. On the next page, we will recreate this using the 960.gs
stylesheet. Instead of writing our own CSS to control layout, we will need
to add classes to the HTML indicating how wide each section should be.
### A Grid-Based Layout Using 960.GS
Let's take a look at an HTML
page and how it has been
marked up to use the 960.gs grid
system.
You can see that we include
the CSS for the grid using the
< link> element inside the
< head> of the page.
