# NextJs: Assets, Metadata, and CSS

The second page we added currently does not have styling. Let's add some CSS to style the page.

Next.js has built-in support for CSS and Sass. For this course, we will use CSS.

This lesson will also talk about how Next.js handles static assets like images and page metadata like the < title> tag.

## Download Starter Code (Optional)
If you’re NOT continuing from the previous lesson, you can download, install, and run the starter code for this lesson below. This sets up a nextjs-blog directory such that it’s identical to the result of the previous lesson.

## Assets
Next.js can serve static assets, like images, under the top-level public directory. Files inside public can be referenced from the root of the application similar to pages.

The public directory is also useful for robots.txt, Google Site Verification, and any other static assets. Check out the documentation for Static File Serving to learn more.


## Image Component and Image Optimization
next/image is an extension of the HTML < img> element, evolved for the modern web.

Next.js also has support for Image Optimization by default. This allows for resizing, optimizing, and serving images in modern formats like WebP when the browser supports it. This avoids shipping large images to devices with a smaller viewport. It also allows Next.js to automatically adopt future image formats and serve them to browsers that support those formats.

## Using the Image Component
Instead of optimizing images at build time, Next.js optimizes images on-demand, as users request them. Unlike static site generators and static-only solutions, your build times aren't increased, whether shipping 10 images or 10 million images.

Images are lazy loaded by default. That means your page speed isn't penalized for images outside the viewport. Images load as they are scrolled into viewport.

## Metadata
What if we wanted to modify the metadata of the page, such as the < title> HTML tag?

< title> is part of the < head> HTML tag, so let's dive into how we can modify the < head> tag in a Next.js page.

## Third-Party JavaScript
Third-party JavaScript refers to any scripts that are added from a third-party source. Usually, third-party scripts are included in order to introduce newer functionality into a site that does not need to be written from scratch, such as analytics, ads, and customer support widgets.

# React Context for Beginners

React context is an essential tool for every React developer to know. I lets you easily share state in your applications.

In this comprehensive guide, we will cover what React context is, how to use it, when and when not to use context, and lots more.


## What is React context?
React context allows us to pass down and use (consume) data in whatever component we need in our React app without using props.

In other words, React context allows us to share data (state) across our components more easily.

## When should you use React context?
React context is great when you are passing data that can be used in any component in your application.

These types of data include:

- Theme data (like dark or light mode)
- User data (the currently authenticated user)
- Location-specific data (like user language or locale)
Data should be placed on React context that does not need to be updated often.

## How do I use React context?
Context is an API that is built into React, starting from React version 16.

This means that we can create and use context directly by importing React in any React project.






