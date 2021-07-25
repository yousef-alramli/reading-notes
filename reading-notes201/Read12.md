# Chart.js, Canvas
![](https://i.stack.imgur.com/RdXEu.png)
## Basic usage of canvas

### <canvas> element
At first sight a  canvas> looks like the < img> element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the < canvas> element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.

### Fallback content
The < canvas> element differs from an < img> tag in that, like for < video>, < audio>, or < picture> elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.
 ### The rendering context
The < canvas> element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. In this tutorial, we focus on the 2D rendering context. Other contexts may provide different types of rendering.

## Drawing shapes with canvas
1. The grid  
Before we can start drawing, we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high.

2. Drawing rectangles  
Unlike SVG, < canvas> only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.
3. Drawing paths  
Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:

- First, you create the path.
- Then you use drawing commands to draw into the path.
- Once the path has been created, you can stroke or fill the path to render it.
4. Moving the pen  
One very useful function, which doesn't actually draw anything but becomes part of the path list described above, is the moveTo() function. You can probably best think of this as lifting a pen or pencil from one spot on a piece of paper and placing it on the next.
5. Arcs  
To draw arcs or circles, we use the arc() or arcTo() methods.
6. Bezier and quadratic curves
The next type of paths available are Bézier curves, available in both cubic and quadratic varieties. These are generally used to draw complex organic shapes.
#### Path2D objects
As we have seen in the last example, there can be a series of paths and drawing commands to draw objects onto your canvas. To simplify the code and to improve performance, the Path2D object, available in recent versions of browsers, lets you cache or record these drawing commands. You are able to play back your paths quickly.
## Applying styles and colors
- Colors  
Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.
- Transparency  
In addition to drawing opaque shapes to the canvas, we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.

- Line styles  
There are several properties which allow us to style lines.
- Patterns  
In one of the examples on the previous page, we used a series of loops to create a pattern of images. There is, however, a much simpler method: the createPattern() method.
- Canvas fill rules  
When using fill (or clip and isPointInPath) you can optionally provide a fill rule algorithm by which to determine if a point is inside or outside a path and thus if it gets filled or not. This is useful when a path intersects itself or is nested.

## Drawing text
The canvas rendering context provides two methods to render text:

fillText(text, x, y [, maxWidth])
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
strokeText(text, x, y [, maxWidth])
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
### Styling text
In the examples above we are already making use of the font property to make the text a bit larger than the default size. There are some more properties which let you adjust the way the text gets displayed on the canvas:












