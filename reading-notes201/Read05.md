# Images, Color, Text
## Images
There are many reasons why you might
want to add an image to a web page: you
might want to include a logo, photograph,
illustration, diagram, or chart.  
  
![](https://miro.medium.com/max/3528/1*Q8w9PI58DKjolhl5aDeiOQ.png)

There are several things to consider when selecting and
preparing images for your site, but taking time to get them
right will make it look more attractive and professional.
In this chapter you will learn how to:  
1. **Include an image in your web pages using HTML:**  

A picture can say a thousand words, and great
images help make the difference between an
average-looking site and a really engaging one.    
2.  **Pick which image format to use:**  

If you are building a site from scratch, it is good
practice to create a folder for all of the images
the site uses.  
3.  **Show an image at the right size:**  

You will also often see an < img>
element use two other attributes
that specify its size:  
- height: 
This specifies the height of the
image in pixels.
- width: 
This specifies the width of the
image in pixels.
4. **Optimize an image for use on the web to make pages load faster:**  

Where an image is placed
in the code will affect how it
is displayed. Here are three
examples of image placement
that produce different results:  

+ before a paragraph:  
The paragraph starts on a new
line after the image.
+ inside the start of a
paragraph:  
The first row of text aligns with
the bottom of the image.
+ in the middle of a
paragraph:  
The image is placed between the
words of the paragraph that it
appears in.

### Old Code: Aligning Images Horizontally

*align:*  
 align attribute was
commonly used to indicate how
the other parts of a page should
flow around an image. It has
been removed from HTML5
and new websites should use
CSS to control the alignment of
images.

### Old Code: Aligning Images Vertically

There are three values that the
align attribute can take that
control how the image should
align vertically with the text that
surrounds it:
+ top:  
This aligns the first line of the
surrounding text with the top of
the image.
+ middle:  
This aligns the first line of the
surrounding text with the middle
of the image.
+ bottom:  
This aligns the first line of the
surrounding text with the bottom
of the image.

### Three Rules for Creating Images
1. Save images in the right format:  

Websites mainly use images in
jpeg, gif, or png format. If you
choose the wrong image
format then your image might
not look as sharp as it should
and can make the web page
slower to load.  

2. Save images at  

the right size
You should save the image at
the same width and height it will
appear on the website. If
the image is smaller than the
width or height that you have
specified, the image can be
distorted and stretched. If the
image is larger than the width
and height if you have specified,
the image will take longer to
display on the page.  

3. Use the correct
resolution:  

Computer screens are made up
of dots known as pixels. Images
used on the web are also made
up of tiny dots. Resolution refers
to the number of dots per inch,
and most computer screens only
show web pages at 72 pixels
per inch. So saving images at
a higher resolution results in
images that are larger than
necessary and take longer to
download
 ### Cropping Images
 When cropping images it is important not to
lose valuable information. It is best to source
images that are the correct shape if possible.
### Image Resolution
Images created for the web should be saved at
a resolution of 72 ppi. The higher the resolution
of the image, the larger the size of the file.
### Vector Images
Vector images differ from bitmap images and
are resolution-independent. Vector images are
commonly created in programs such as Adobe
Illustrator.
### Transparency
Creating an image that is partially transparent
(or "see-through") for the web involves
selecting one of two formats:
1. Transparent GIF
2. PNG

### HTML 5: Figure and Figure Caption
  
< figure>
Images often come with
captions. HTML5 has introduced
a new < figure> element to
contain images and their caption
so that the two are associated.

The < figcaption> element has
been added to HTML5 in order
to allow web page authors to add
a caption to an image.

## Color
Color can really bring your pages to life.
In this chapter we will look at:

- How to specify colors, as there are three common ways in
which you can indicate your choice of colors (plus extra
ways made available in CSS3)
- Color terminology, as there are some terms that are very
helpful to understand when it comes to picking colors
-  Contrast, and ensuring that your text is readable
-  Background colors for behind either your entire page or
parts of a page


### Foreground Color
The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:
- rgb values  
These express colors in terms
of how much red, green and
blue are used to make it up. For
example: rgb(100,100,90)

- hex codes  
These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80

- color names  
There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCyan-

### Background Color
CSS treats each HTML element
as if it appears in a box, and the
background-color property
sets the color of the background
for that box.

### Contrast
When picking foreground and background
colors, it is important to ensure that there is
enough contrast for the text to be legible.
### CSS 3: Opacity

CSS3 introduces the opacity
property which allows you to
specify the opacity of an element
and any of its child elements.
The value is a number between
0.0 and 1.0 (so a value of 0.5
is 50% opacity and 0.15 is 15%
opacity).

### CSS 3: HSL & HSLA
The hsl color property has
been introduced in CSS3 as an
alternative way to specify colors.
The value of the property starts
with the letters hsl, followed
by individual values inside
parentheses for:  
- hue  
This is expressed as an angle
(between 0 and 360 degrees).
- saturation  
This is expressed as a
percentage.
- lightness  
This is expressed as a
percentage with 0% being white,
50% being normal, and 100%
being black.

## Text
The properties that allow you to control
the appearance of text can be split into
two groups:  
- Those that directly affect the font and its appearance
(including the typeface, whether it is regular, bold or italic,
and the size of the text)
- Those that would have the same effect on text no matter
what font you were using (including the color of text and
the spacing between words and letters)
### Typeface Terminology
- Serif
Serif fonts have extra details on
the ends of the main strokes of
the letters. These details are
known as serifs.
- Sans-Serif
Sans-serif fonts have straight
ends to letters, and therefore
have a much cleaner design.
- small 
sans-serif fonts can be clearer
to read.
Monospace
Every letter in a monospace (or
fixed-width) font is the same
width. (Non-monospace fonts
have different widths.)

### Choosing a Typeface for your Website
When choosing
a typeface, it
is important to
understand that a
browser will usually
only display it if it's
installed on that
user's computer.
### Techniques That Offer a Wider Choice of Typefaces
There are several ways to use fonts other than those listed on the
previous page. However, typefaces are subject to copyright, so the
techniques you can choose from are limited by their respective licenses.
### Specifying Typefaces
The font-family property
allows you to specify the
typeface that should be used for
any text inside the element(s) to
which a CSS rule applies.
### Size of Type
The font-size property enables
you to specify a size for the
font. There are several ways to
specify the size of a font.

### Type Scales
The default size of text in a
browser is 16 pixels. So if you
use percentages or ems, you
calculate the size of text you
want based on the default size
of the text used in browsers.
For example, you could scale
down to 12 pixels for body copy
and scale up to 24 pixels for
headings.

### Units of Type Size
- Pixels  
Setting font size in pixels is the
best way to ensure that the type
appears at the size you intended
(because percentages and ems
are more likely to vary if a user
has changed the default size of
text in their browser).
- Percentages  
The default size of text in a
web browser is 16 pixels. Using
percentages of this amount, you
can create a scale where the
default text size is 12 pixels, and
headings are sized in relation
to this.
- Ems  
Ems allow you to change the size
of text relative to the size of the
text in the parent element. Since
the default size of text in web
browsers is 16 pixels, you can
use similar rules to those shown
for percentages.

### Underst anding Font Formats
Different browsers support
different formats for fonts
(in the same way that they
support different audio and
video formats), so you will need
to supply the font in several
variations to reach all browsers.
### CSS3: Drop Shadow
The text-shadow property has
become commonly used despite
lacking support in all browsers.
It is used to create a drop
shadow, which is a dark version
of the word just behind it and
slightly offset. It can also be used
to create an embossed effect by
adding a shadow that is slightly
lighter than the text.
### First Lett er or Line
You can specify different values
for the first letter or first line of
text inside an element using
:first-letter and
:first-line.
### Responding to Users
- :hover
This is applied when a user
hovers over an element with a
pointing device such as a mouse.
This has commonly been used
to change the appearance of
links and buttons when a user
places their cursor over them. It
is worth noting that such events
do not work on devices that use
touch screens (such as the iPad)
because the screen is not able to
tell when someone is hovering
their finger over an element.
- :active
This is applied when an element
is being activated by a user; for
example, when a button is being
pressed or a link being clicked.
Sometimes this is used to make
a button or link feel more like it
is being pressed by changing the
style or position of the element
slightly.
- :focus
This is applied when an element
has focus. Any element that
you can interact with, such as a
link you can click on or any form
control can have focus.
### Att ribute Selectors
You met the most popular CSS selectors on page 238. There are also
a set of attribute selectors that allow you to create rules that apply to
elements that have an attribute with a specific value.
## JPEG vs PNG vs GIF
### TL;DR
+ Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth.
+ Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos.
+ Use GIF format for images that contain animations.
### Compression
- *JPEG:*  
 is a lossy compression specification that takes advantage of human perception. It can achieve compression ratios of 1:10 without any perceivable difference in quality. Beyond this, the compression artefacts become more prominent. Because JPEG compression works by averaging out colours of nearby pixels (read Discrete Cosine Transform), JPEG images are best suited for photographs and paintings of natural scenes where the variations in colour and intensity are smooth. However, if an image contains text or lines, where a sharp contrast between adjacent pixels is desired to highlight the proper shape, this lossy compression technique does not yield good results.
- *PNG:*  
 is a lossless image format using DEFLATE compression. No data is lost during compression and no compression artefacts are introduced in the image. For this reason, a PNG image would retain higher quality than an image than JPEG and would look a lot sharper, it would also occupy more space on the disk. This makes it unsuitable for storing or transferring high-resolution digital photographs but a great choice for images with text, logos and shapes with sharp edges.

- *GIF:*   
is also a lossless image format that uses LZW compression algorithm. It was favoured over PNG for simple graphics in websites in its early days because the support of PNG was still growing. Given that PNG is now supported across all major devices and that PNG compression is about 5–25% better than GIF compression, GIF images are now mainly used only if the image contains animations.
 
### Transparency
- JPEG images don’t support transparency and are hence not usable for such cases.
- GIF images support transparency by declaring a single colour in the colour palette as transparent (index transparency).
- PNG images support transparency in two ways — inserting an alpha channel that allows partial transparency or by declaring a single colour as transparent (index transparency).



