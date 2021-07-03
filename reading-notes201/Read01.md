# Introductory HTML and JavaScript Summary
## Introduction of HTML
#### the different ways in which people access the web :

1. **Browses**  
   Websites can be accessed by
   software called a web browser (EX. Firefox, Internet Explorer, Safari, Chrome, and Opera).  
  

2. **Web Servers**  
   When you ask your browser for a web page, the request is sent across the Internet to **web Server**.  
   **Web Servers** are special computers that are constantly
   Connected to the Internet, and are optimized to send web pages
   out to people when request them.  
   Some big companies run their
   own web servers, but it is more
   common to use the services of
   a web hosting company who
  charge a fee to host your site.

3. **Screen readers**  
   Its programs for the people with visual impairments that read out the contents of a computer screen to the user.

4. **Devices**
   People accesses the internet by a variety of devices with deferent sizes and some have faster connection from others.


#### How Websites Are Created
   All websites use HTML and CSS, but content management systems blogging software, and e-commerce platforms often add a few more technologies into the mix.

  * When you are looking at a website, it is most likely that your browser will be receiving HTML and CSS from the web server that hosts the site. The web browser interprets the HTML and CSS code to create the page that you see, Some sites also send JavaScriptor Flash to your browser.


  * Small websites are often written just using HTML and CSS. Larger websites — in particular those that are updated regularly and use a content management system (CMS), blogging tools, or e-commerce software — often make use of more complex technologies on the web server.


#### How the Web Works
   When you visit a website, the web server hosting that site could be anywhere in the world. In order for you to find the location of the web server, your browser will first connect to a Domain Name System (DNS) server.

**The steps to accsses a website:**  
   1. You type a domain name or web address into your browser to visit a site.  
   2. Your computer contacts Domain Name System (DNS) servers,they tell your computer the IP address associated with the requested domain name.  
   3. IP allows your browser to contact the web server that hosts the website you requested.  
   4. The web server then sends the page you requested back to your web browser.


## Structure
HTM L Describes the Structure of Pages.


**HTML elementsis** are made up of characters that live inside angled brackets, Elements are usually made up of two tags: an opening tag and a closing tag. (The closing tag
has an extra forward slash in it.), HTML elements tells the browser the meaning of information that sits between its opening and closing tags.


#### **  Attributes:**  

Attributes provide additional information
about the contents of an element. They appear
on the opening tag of the element and are
made up of two parts: a name and a value,
separated by an equals sign.

- The attribute name indicates
what kind of extra information
you are supplying about the
element's content. It should be
written in lowercase.
- Attribute should be placed in double
quotes. Different attributes can
have different values.
- The majority of attributes can
only be used on certain
elements, although a few
attributes (such as lang)
can appear on any element.
- Most attribute values are
either pre-deﬁned or follow a
stipulated format.


## Extra Markup


#### The Evolution of HTML

Since the web was first created, there have
been several different versions of HTML.

Each new version was designed
to be an improvement on the
last (with new elements and
attributes added and older code removed).
There have also been several versions of each browser used to view web pages, each of which implements new code.

*examples of HTML version:*  

- HTML 4 Released 1997: HTML 4 had some
presentational elements to
control the appearance of pages.
- XHTML 1.0 Released 2000:in 1998, a language called XML was published. Its purpose was to allow people to write new markup languages.
- HTML5 Released 2000: In HTML5, web page authors do not need to close all tags, and new elements and attributes will be introduced.

#### DOCTYPEs

Because there have been several versions of HTML, each web page should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using (although browsers usually display the page even if it is not included).

#### Commentsin HTML

If you want to add a comment to your code that will not be visible in the user's browser, you can add the text between these characters:  <!-- comment -->  


comments are not visible to users in the main browser window, they can be viewed by anyone who looks at the source code behind the page.

Comments can also be used around blocks of code to stop that code from being displayed in the browser.

#### ID Attribute
Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page. Its value should start with a letter or an underscore (not a number or any other character).
When you come to look at CSS in the next section, giving an element a unique identity allows you to style it differently than any other instance of the same element on the page.
- The id attribute is known as a **global attribute** because it can be used on any element.

#### Class Attribute

Every HTML element can also carry a class attribute.
Sometimes, rather than uniquely identifying one element within a document, you will want a
way to identify several elements as being different from the other elements on the page.  
To do this you can use the class attribute. Its value should describe the class it belongs to.

#### Block Elements

block level is the elements that will always appear to start on a new line in the browser window.  
Examples of block elements are <h1>, <p>, <ul>, and <li>.

#### Inline Elements

inline elements are the elements that will always appear to continue on the same line as their neighbouring elements.
Examples of inline elements are <a>, <b>, <em>, and <img>.

#### Grouping Text & Elements In a Block


 ##### **<div> **
 

The <div> element allows you to
group a set of elements together
in one block-level box.  
In a browser, the contents of the <div> element will start on a new line, but other than this it will make no difference to the presentation of the page.

 ##### **<span> **
 The <span> element acts like an inline equivalent of the <div> element.

 It is used to either:  
1. Contain a section of text where there is no other suitable element to differentiate it from its surrounding text.  
2. Contain a number of inline elements.  

The most common reason why people use <span> elements is so that they can control the appearance of the content of these elements using CSS.

####  IFrames

##### <iframe> 
An iframe is like a little window that has been cut into your page — and in that window you can see another page. The term iframe is an abbreviation of inline frame.

There are a few attributes that you will need to know to use it:  


* src

The src attribute specifies the URL of the page to show in the frame.
* height

The height attribute specifies
the height of the iframe in pixels.
* width

The width attribute specifies the width of the iframe in pixels.

* scrolling

The scrolling attribute will
not be supported in HTML5. In
HTML 4 and XHTML, it indicates
whether the iframe should
have scrollbars or not. Scrollbars allow the user to move
around the frame to see more content. It can take one of three values:   
1. yes (to show scrollbars)  
2. no (to hide scrollbars)  
3. auto (to show them only if needed).

* frameborder

The frameborder attribute will
not be supported in HTML5. In
HTML 4 and XHTML, it indicates
whether the frame should have
a border or not. 
* seamless

In HTML5, a new attribute
called seamless can be applied
to an iframe where scrollbars
are not desired. The seamless
attribute (like some other new
HTML5 attributes) does not
need a value, but you will often
see authors give it a value of
seamless.


#### Information About Pages
##### <meta>

The <meta> element lives
inside the <head> element and
contains information about that
web page.  
The <meta> element is an empty
element so it does not have a
closing tag. It uses attributes to
carry the information.

#### Escape Characters


There are some characters that are used in and reserved by HTML code.  

Therefore, if you want these
characters to appear on your
page you need to use what are
termed "escape" characters
(also known as escape codes or
entity references). For example,
to write a left angled bracket,
you can use either &lt; or
&#60;. For an ampersand, you
can use either &amp; or &#38;.

There are also special codes
that can be used to show
symbols such as copyright and
trademark, currency symbols,
mathematical characters, and
some punctuation marks. For
example, if you want to include a
copyright symbol on a web page
you can use either &cop y; or
& #169;.

## HTML5 Layout

#### Traditional HTML Layouts
For a long time, web page authors used <div> elements to group
together related elements on the page. Authors used class or id attributes to indicate the role of the <div> element in the structure of the page.

#### New Html 5 Layout Elements
HTML5 introduces a new set of elements that allow you to divide up the parts of a page. The names of these elements indicate the kind of content you will find in them. They are still subject to change, but that has not stopped many web page authors using them already.
 
 #### Headers & Footers

 The <header> and <footer> elements can be used for:

- The main header or footer that appears at the top or bottom of every page on the site.
- A header or footer for an individual <article> or <section> within the page.

#### Navigation
The <nav> element is used to
contain the major navigational
blocks on the site such as the
primary site navigation.


#### Articles

The <article> element acts as a container for any section of a page that could stand alone and potentially be syndicated.

#### Aside

The <aside> element has two purposes, depending on whether it is inside an <article> element or not.

- When the <aside> element
is used inside an <article>
element, it should contain
information that is related to the
article but not essential to its
overall meaning.
- When the <aside> element is
used outside of an <article>
element, it acts as a container
for content that is related to
the entire page.

#### Sections
The <section> element groups
related content together, and
typically each section would
have its own heading.  

The <section> element should
not be used as a wrapper for
the entire page (unless the
page only contains one distinct
piece of content). If you want a
containing element for the entire
page, that job is still best left to
the <div> element.

#### Heading Groups
The purpose of the <hgroup>
element is to group together a
set of one or more <h1> through
<h6> elements so that they are
treated as one single heading.

#### Figures

<figure> can be used
to contain any content that is
referenced from the main flow of
an article (not just images).

it should only be
used when the content simply
references the element.

Examples of usage include:
- Images
- Videos
- Graphs
- Diagrams
- Code samples
- Text that supports the main body of an article.


The <figure> element should
also contain a <figcaption>
element which provides a text
decription for the content of
the <figure> element.

#### Sectioning El ements

the <div> element
will remain an important way to
group together related elements,
because you should not be using
these new elements that you
have just met for purposes other
than those explicitly stated.

#### Linking Around Block-Level Elements


HTML5 allows web page authors
to place an <a> element around
a block level element that
contains child elements. This
allows you to turn an entire block
into a link.

#### Helping Older Browsers Understand

Older browsers that do not
know the new HTML5 elements
will automatically treat them as
inline elements. Therefore, to
help older browsers, you should
include the line of CSS on the
left which states which new
elements should be rendered as
block-level elements.


## Process & Design

Every website should be designed for the
target audience—not just for yourself or the
site owner. It is therefore very important to
understand who your target audience is.

Target Audience: individuals

- f your target audience?
- Will your site appeal to more women or men? What is the mix?
- Which country do your visitors live in?
- Do they live in urban or rural areas?
- What is the average income of visitors?
- What level of education do they have?
- What is their marital or family status?
- What is their occupation?
- How many hours do they work per week?
- How often do they use the web?
- What kind of device do they use to access the web?

Target Audience: Companies

- What is the size of the company or relevant department?
- What is the position of people in the company who visit your site?
- Will visitors be using the site for themselves or for someone else?
- How large is the budget they control?

Invent some fictional visitors from your typical
target audience. They will become your friends.
They can influence design decisions from color
palettes to level of detail in descriptions.


#### Why People Visit YOUR Website

Now that you know who your visitors are, you
need to consider why they are coming. While
some people will simply chance across your
website, most will visit for a specific reason.


Key Motivations:

* Are they looking for general entertainment or do they need to achieve a specific goal?
* If there is a specific goal, is
it a personal or professional
one?
* Do they see spending time on
this activity as essential or a
luxury?

Specific Goals:

* Do they want general
information / research (such
as background on a topic /
company), or are they after
something specific (such as a
particular fact or information
on a product)?
* Are they already familiar with
the service or product that
you offer or do they need to
be introduced to it?
* Are they looking for time
sensitive information, such as
the latest news or updates on
a particular topic?
* Do they want to discover
information about a specific
product or service to help
them decide whether to buy
it or not?
* Do they need to contact you?
If so, can they visit in person
(which might require opening
hours and a map)? Or might
they need email or telephone
contact details?

#### What Your Visitors are Trying to Achieve

First you want to create a list
of reasons why people would
be coming to your site. You can
then assign the list of tasks to
the fictional visitors you created
in the step described on the
previous page.

#### What Information Your Visitors Need

You know who is coming to your site and why
they are coming, so now you need to work out
what information they need in order to achieve
their goals quickly and effectively.

#### How Of ten People Will Visit Your Site

Some sites benefit from being updated more
frequently than others. Some information (such
as news) may be constantly changing, while
other content remains relatively static.

#### Site Maps

Now that you know what needs to appear
on your site, you can start to organize the
information into sections or pages.
![site map](https://cdn.shortpixel.ai/client/q_lqip,ret_wait,w_440,h_215/https://blog.mindmanager.com/wp-content/uploads/sites/6/2011/03/web_sitemap_expl4.jpeg)

The aim is to create a diagram
of the pages that will be used
to structure the site. This is
known as a site map and it will
show how those pages can be
grouped.

#### WireFrames

A wireframe is a simple sketch of the key
information that needs to go on each page of a
site. It shows the hierarchy of the information
and how much space it might require.

A lot of designers will take the
elements that need to appear on
each page and start by creating
wireframes. This involves
sketching or shading areas
where each element of the page
will go (such as the logo, primary
navigation, headings and main
bodies of text, user logins etc).

![](https://cacoo.com/wp-app/uploads/2018/10/Cacoo-8-must-see-wireframes-680x450.png)



 #### Getting your message across using design

The primary aim of any kind of visual design
is to communicate. Organizing and prioritizing
information on a page helps users understand
its importance and what order to read it in.

- CONTENT:  
Web pages often have a lot of
information to communicate.
- Prioritizing:  
If everything on a page appeared
in the same style, it would be
much harder to understand. (Key
messages would not stand out.)

- Organizing:  
Grouping together related
content into blocks or chunks
makes the page look simpler
(and easier to understand).

#### Visual Hierarchy
Most web users do not read entire pages. Rather, they skim to find
information. You can use contrast to create a visual hierarchy that gets
across your key message and helps users find what they are looking for.

- SIZE  
Larger elements will grab users'
attention first. For this reason it
is a good idea to make headings
and key points relatively large.
- COLOR  
Foreground and background
color can draw attention to key
messages. Brighter sections tend
to draw users' attention first.
- Style  
An element may be the same
size and color as surrounding
content but have a different style
applied to it to make it stand out.

**Visual hierarchy** refers to the order in which your eyes perceive what
they see. It is created by adding visual contrast between the items being
displayed. Items with higher contrast are recognized and processed first.

#### grouping and Similarity

When making sense of a design, we tend to organize visual elements
into groups. Grouping related pieces of information together can make a
design easier to comprehend. Here are some ways this can be achieved.

+ Proximity  
When several items are
placed close together, they are
perceived as more related than
items that are placed further
apart. (You can also nest groups
of information within larger
groups of information.)
+ Closure  
When faced with a complicated
arrangement of items, we
will often look for a single or
recognisable pattern or form.
A real or imaginary box can be
formed around elements due to
their proximity and alignment.
+ Continuance  
When elements are placed in
a line or a curve then they are
perceived to be more related
than those that are not following
the same direction. This can be
used to direct a reader from one
part of a page to the next.
+ White Space  
Placing related items closer
together and leaving a bigger
gap between unrelated items.
+ color  
A background color placed
behind related items to
emphasize their connection.
+ Borders  
A line can be drawn around the
border of the group or between it
and its neighbors.
 
#### Designing Navigation

Site navigation not only helps people find where they want to go, but also helps them understand what your site is about and how it is organized.  
Good navigation tends to follow these principles:

- Concise  
Ideally, the navigation should
be quick and easy to read. It is
a good idea to try to limit the
number of options in a menu to
no more than eight links. These
can link to section homepages
which in turn link to other pages.
- Clear  
Users should be able to predict
the kind of information that
they will find on the page
before clicking on the link.
Where possible, choose single
descriptive words for each link
rather than phrases.
- Selective  
The primary navigation should
only reflect the sections or
content of the site. Functions
like logins and search, and legal
information like terms and
conditions and so on are best
placed elsewhere on the page.

+ Context  
Good navigation provides
context. It lets the user know
where they are in the website at
that moment. Using a different
color or some kind of visual
marker to indicate the current
page is a good way to do this.
+ Interactive  
Each link should be big enough
to click on and the appearance
of the link should change when
the user hovers over each item
or clicks on it. It should also
be visually distinct from other
content on the page.
+ Consistent  
The more pages a site contains,
the larger the number of
navigation items there will be.
Although secondary navigation
will change from page to page,
it is best to keep the primary
navigation exactly the same.

## Introduction of JavaScript

JavaScript is a programming language we can use to make a website interactive. 

#### ACCESS CONTENT
You can use JavaScript to select any
element, attribute, or text from an
HTML page. For example:
+ Select the text inside all of the <hl>
elements on a page
+ Select any elements that have a
class attribute with a value of note
+ Find out what was entered into a
text input whose id attribute has a
value of email 
#### MODIFY CONTENT
You can use JavaScript to add
elements, attributes, and text to the
page, or remove them. For example:
+ Add a paragraph of text after the
first <hl> element
+ Change the value of class
attributes to trigger new CSS rules
for those elements
+ Change the size or position of an
<i mg> element

#### PROGRAM RULES
You can specify a set of steps for
the browser to follow (like a recipe),
which allows it to access or change the
content of a page. For example:
- A gallery script could check which
image a user clicked on and display
a larger version of that image.
- A mortgage calculator could collect
values from a fo rm, perform a
ca lculation, and display repayments.
- An animation could check the
dimensions of the browser window
and move an image to the bottom
of the viewable area (also known as
the viewport).
#### REACT TO EVENTS
You can specify that a script should run
when a specific event has occurred. For
example, it could be run when:
- A button is pressed
- A link is clicked (or tapped) on
- A cursor hovers over an element
- Information is added to a form
- An interval of time has passed
- A web page has finished loading

### EXAMPLES OF JAVASCRIPT
IN THE BROWSER
Being able to change the content of an HTML page while it is loaded in the browser is very powerful. 

The examples below rely on the ability to:  
**Access** the content of the page   
**Modify** the content of the page  
**Program rules** or instructions the browser can follow  
**React** to events triggered by the user or browser  

## The ABC of Programming

### What Is Script and How Do I Creat One  

A script is a series of instructions that a
computer can follow to achieve a goal.  

#### WRITING A SCRIPT

To write a script, you need to first
state your goal and then list the
tasks that need to be completed in
order to achieve it.

Start with the big picture of what you want to achieve, and break that down into smaller steps.  

1. DEFINE THE GOAL
First, you need to define the task you want to
achieve. You can think of this as a puzzle for the
computer to solve.  

2. DESIGN THE SCRIPT  
To design a script you split the goal out into a series
of tasks that are going to be involved in solving this
puzzle. This can be represented using a flowchart.
You can then write down individual steps that the
computer needs to perform in order to complete
each individual task (and any information it needs to
perform the task), rather like writing a recipe that it
can follow.  

3. CODE EACH STEP  
Each of the steps needs to be written in a
programming language that the compu ter
understands. In our case, this is JavaScript.


#### Design Script 

steps:

- You start with an idea.
- Pre-write.
- Build your world.
- Set your characters, conflict, and relationships.
- Write – synopsis, treatment, and then the script itself.
- Write in format.
- Rewrite.
- Submit.

#### FROM STEPS TO CODE

Just like learning any new language, you need
to get to grips with the:  
- Vocabulary: The words that computers
understand
- Syntax: How you put those words together to
create instructions computers can follow.

#### DEFINING A GOAL & DESIGNING THE SCRIPT

Consider how you might approach a different type of script.
This example calculates the cost of a name plaque.
Customers are charged by the letter.

#### SKETCHING OUT THE TASKS IN A FLOWCHART

Often scripts will need to perform different tasks in different situations.
You can use flowcharts to work out how the tasks fit together.
The flowcharts show the paths between each step.

### how do cumputers fit in with the world 

#### COMPUTERS CREATE MODELS OF THE WORLD
USING DATA
Here is a model of a hotel, along with some model trees, model people,
and model cars. To a human, it is clear what kind of real -world object
each one represents.

#### OBJECTS & PROPERTIES
OBJECTS (THINGS)
In computer programming, each physica l thing in
the world can be represented as an object. There are
two different types of objects here: a hotel and a car.
Programmers might say that there is one instance of
the hotel object, and two instances of the car object.
Each object can have its own:
- Properties
- Events
- Methods

#### EVENTS
In the real world, people interact with objects. These interactions can
change the values of the properties in these objects.
WHAT IS AN EVENT?
There are common ways in which people interact
with each type of object.  
 For example, in a car a
driver will typically use at least two pedals. The car
has been designed to respond differently when the
driver interacts with each of the different pedals:
- The accelerator makes the car go faster
- The brake slows it down

#### METHODS
Methods represent things people need to do with objects. They can
retrieve or update the values of an object's properties.
WHAT IS A METHOD?
Methods typically represent how people (or other
things) interact with an object in the real world.

They are like questions and instructions that:  
- Tell you something about that object (using
information stored in its properties)
- Change the value of one or more of that object's
properties

#### PUTTING IT ALL TOGETHER
Computers use data to create models of things in the real world.
The events, methods, and properties of an object all relate to each other:
Events can trigger methods, and methods can retrieve or update an
object's properties.


#### WEB BROWSERS ARE PROGRAMS BUILT USING OBJECTS

You have seen how data can be used to create a model of a hotel or a car.
Web browsers create similar models of the web page they are showing
and of the browser window that the page is being shown in.

**WINDOW OBJECT**  
On the right-hand page you can see a model of a
computer with a browser open on the screen.
The browser represents each window or tab using a
window object. The location property of the window
object will tell you the URL of the current page.

#### THE DOCUMENT OBJECT REPRESENTS AN HTML PAGE

Using the document object, you can access and change what content
users see on the page and respond to how they interact with it.
Like other objects that represent real-world things,
the document object has:
- PROPERTIES  
Properties describe characteristics of the current
web page (such as the t itle of the page).
- METHODS  
Methods perform tasks associated with the
document currently loaded in the browser (such
as getting information from a specified element or
adding new content).
- EVENTS  
You can respond to events, such as a user clicking or
tapping on an element.

#### HOW A BROWSER SEES A WEB PAGE


- RECEIVE A PAGE AS  
HTML CODE
Each page on a website can be
seen as a separate document .
So, the web consists of many
sites, each made up of one or
more documents.

- CREATE A MODEL OF  
THE PAGE AND STORE
IT IN MEMORY
The model shown on the right
hand page is a representation
of one very basic page. Its
structure is reminiscent of a
family tree. At the top of the
model is a document object,
which represents the whole
document.

- USE A RENDERING  
ENGINE TO SHOW THE
PAGE ON SCREEN
If there is no CSS, the rendering
engine will apply default styles
to HTML elements. However,
the HTML code for this example
links to a CSS style sheet, so the
browser requests that file and
displays the page accordingly.


All major browsers use a JavaScript interpreter to translate your
instructions (in JavaScript) into instructions the computer can follow.

### How Do I Script For aWeb Page 

#### HOW HTML, CSS, & JAVASCRIPT FIT TOGETHER

Before diving into the JavaScript language, you
need to know how it will fit together with the
HTML and CSS in your web pages.

- CONTENT LAYER
. html files  
This is where the content of
the page lives. The HTML gives
the page structure and adds
semantics.

- PRESENTATION LAYER
.css files  
The CSS enhances the HTML
page with rules that state how
the HTML content is presented
(backgrounds, borders, box
dimensions, colors, fonts, etc.).

- BEHAVIOR LAYER .js files  
This is where we can change
how the page behaves, adding
interact ivity. We will aim to keep
as much of our JavaScript as
possible in separate files.

#### PROGRESSIVE ENHANCEMENT


These three layers form the basis of a popular
approach to building web pages called
progressive enhancement.

* HTML ONLY  
Starting with the HTML layer
allows you to focus on the most
important thing about your site:
its content.

* HTML+CSS  
Adding the CSS rules in a
separate file keeps rules
regarding how the page looks
away from the content itself.
 * HTML+CSS+JAVASCRIPT  
The JavaScript is added last
and enhances the usability of
the page or the experience of
interacting with the site.

#### CREATING A BASIC JAVASCRIPT

JavaScript is written in plain text, just like HTML and CSS, so you do not
need any new tools to write a script. This example adds a greeting into an
HTML page. The greeting changes depending on the time of day.

#### LINKING TO A JAVASCRIPT FILE FROM AN HTML PAGE
When you want to use JavaScript with a web page, you use the HTML
<script> element to tell the browser it is coming across a script.
Its s re attribute tells people where the JavaScript file is stored.








