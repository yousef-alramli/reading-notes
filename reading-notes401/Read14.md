# Matplotlib tutorial
**Matplotlib** is a multi-platform data visualization library built on NumPy arrays, and designed to work with the broader SciPy stack. It was conceived by John Hunter in 2002, originally as a patch to IPython for enabling interactive MATLAB-style plotting via gnuplot from the IPython command line.

### IPython
IPython is an interactive shell that is built with python. It provides a more useful shell environment to execute python code in REPL (Read Eval Print Loop). 

### pyplot
pyplot is a state-based interface to matplotlib. It provides a MATLAB-like way of plotting. pyplot is mainly intended for interactive plots and simple cases of programmatic plot generation.

## Simple plot
The **simple plot** is defined as a unified construct of necessary and probable actions accompanied by a change of fortune. Change of fortune is a crucial aspect of this type of plot — particularly the word change.

## Figures, Subplots, Axes and Ticks

### Figures
A figure is the windows in the GUI that has "Figure #" as title. Figures are numbered starting from 1 as opposed to the normal Python way starting from 0. This is clearly MATLAB-style.

### Subplots
Subplots are groups of axes that can exist in a single matplotlib figure. subplots() function in the matplotlib library, helps in creating multiple layouts of subplots. It provides control over all the individual plots that are created. Matplotlib Subplots in Python.

### Axes
Axes object is the region of the image with the data space. A given figure can contain many Axes, but a given Axes object can only be in one Figure. The Axes contains two (or three in the case of 3D) Axis objects.

### Ticks
Ticks are the values used to show specific points on the coordinate axis. It can be a number or a string. Whenever we plot a graph, the axes adjust and take the default ticks. Matplotlib's default ticks are generally sufficient in common situations but are in no way optimal for every plot.

## Animation
For quite a long time, animation in matplotlib was not an easy task and was done mainly through clever hacks. However, things have started to change since version 1.1 and the introduction of tools for creating animation very intuitively, with the possibility to save them in all kind of formats (but don't expect to be able to run very complex animations at 60 fps though).
- Drip drop
- Earthquakes
- Scatter Plots
- Bar Plots
- Contour Plots
- Imshow
- Pie Charts
- Quiver Plots
- Multi Plots
- Polar Axis
- 3D Plots
- Text


# Bokeh Tutorial

## What is Bokeh

Bokeh is an interactive visualization library that targets modern web browsers for presentation. It is good for:

* Interactive visualization in modern browsers
* Standalone HTML documents, or server-backed apps
* Expressive and versatile graphics
* Large, dynamic or streaming data
* Easy usage from python (or Scala, or R, or...)

And most importantly: **NO JAVASCRIPT REQUIRED**

Bokeh is an interactive visualization library for modern web browsers. It provides elegant, concise construction of versatile graphics, and affords high-performance interactivity over large or streaming datasets. Bokeh can help anyone who would like to quickly and easily make interactive plots, dashboards, and data applications.



