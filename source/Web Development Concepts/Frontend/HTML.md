---
layout: default
title: Hypertext Markup Language
nav_order: 1
permalink: Web Development Concepts/Frontend/HTML
grand_parent: Web Development Concepts
parent: Frontend
has_children: false
---

# What is Hypertext Markup Language (HTML)?
{: .no_toc }

{: .note }

HTML serves as the building blocks for our website. It represents the different pieces for your LEGO figure, the head, arms, body, legs.

Every HTML page ends with ".html", where each page has the same starting structure. The `<head>` contains all of the "metadata" which are information related to the website. The actual content goes inside of the `<body>`tags.

```
<!doctype html>
<html lang="en-US">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width" />

    <title>My page title</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body></body> <!--The actual content goes inside the <body> tags--> 
</html>
```

Most HTML tags are structured like this:

![](https://clearlydecoded.com/assets/images/posts/2017-09-04-anatomy-of-html-tag/html-tag-attributes.png)

One important aspect of HTML is **the DOM**

**The DOM, or Document Object Model**, is like the instruction manual that tells you how to put all those LEGO bricks together to build your house.

The web browser is like a really smart LEGO builder. When you open a web page, the browser starts reading through that instruction manual, the HTML code.

The DOM is like a map of your web page, showing how all these HTML elements are connected and organized. It's a way for your web browser to understand the structure of your page so it knows how to display it properly. 

It's like a blueprint of the web page, showing how all the HTML elements are connected and organized, just like how the instruction manual tells the builder how to connect all the LEGO bricks to build the house.

Just like how following the LEGO instruction manual helps you build your house correctly, the DOM helps the web browser render your web page correctly, making sure everything shows up in the right place and looks the way it should.

The browser knows exactly where everything is on the page because it's already built that LEGO-like map in its memory using the DOM. This helps the browser quickly find and update different parts of the web page without getting confused, just like how a LEGO builder can quickly find and add or remove bricks from the right spots in the house they're building!

**To learn more about HTML, down below are some resources:**

[HTML on W3Schools](https://www.w3schools.com/html)
[Mozilla HTML Documentation](https://developer.mozilla.org/en-US/docs/Web/HTML)


[Previous: Frontend](../Frontend){: .float-left .v-align-text-top}
[Next: CSS](CSS){: .float-right .v-align-text-top}
