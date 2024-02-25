---
layout: default
title: Cascading Style Sheets
nav_order: 2
permalink: Web Development Concepts/Frontend/CSS
grand_parent: Web Development Concepts
parent: Frontend
has_children: false
---

# What are Cascading Style Sheets (CSS)?
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

{: .note }
> By [Victor Hsiao](https://www.linkedin.com/in/hsiaovictor/)    

CSS, or Cascading Style Sheets, is like the paint and decorations you use to make your LEGO house look awesome after you've built it. While HTML defines the structure and content of your web page, CSS controls how your web page looks, like the colors, fonts, sizes, and layout.

CSS works together with HTML to make your web page look fantastic. It's like adding all the cool paint colors, decorations, and designs to your LEGO house after you've built it. You use CSS to tell the browser how you want each part of your web page to look.

For example, you can use CSS to make your headings big and bold, your paragraphs have a specific font, and your buttons stand out with a bright color. HTML tells the browser what content goes where, and CSS tells the browser how to style and present that content, just like how the instructions tell you where to put each LEGO brick and the decorations to make your house look amazing. 

Together, HTML and CSS work hand in hand to create beautiful and functional web pages, just like how LEGO bricks and decorations come together to make awesome creations!

## Types of Styling

There are different types of CSS styling you can implement:

### **Inline Styling**

Inline styling is when you add CSS styles inside an HTML tag

To do inline styling, you add the  `style` attribute inside an HTML tag, and then the specific CSS property inside the quotes of the style attribute, only do styling within the `<body>` tag, and inside the opening tag only (not in the closing tag)

`<h1 style="color:red">Hello!</h1>`

This is considered the most inefficient form of implementing CSS styles because if we want to implement multiple CSS properties, it can get pretty jumbled and messy!

### **Internal Styling**

To utilize internal styling, you add the `<style>` element inside the `<head>` section

```
<!DOCTYPE html>
<html>
<head>
<style>
body {background-color: powderblue;}
h1   {color: blue;}
p    {color: red;}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

This separates the CSS from the HTML code and makes it easier to read when multiple styles are implemented for a specific element. However, we want to keep our HTML and CSS code separate from each other, and the best way is to keep the HTML and CSS code in separate files

### **External Styling**

For external CSS styling, we use the ```<link>``` tag, which we add to the ```<head>``` section in our HTML

```<link rel="stylesheet" href="(name of css file).css" />```

We add the rel attribute and specify it as a "stylesheet" to specify that we want to add CSS code to our HTML, and then the href attribute to link our CSS code to the HTML

Overall, CSS can make our website look pretty and stylish. Like with our LEGO house, we can use CSS to make our website stand out in its own unique way!
_______________________________________________________________

[Previous: HTML](HTML){: .float-left .v-align-text-top}
[Next: Javascript](Javascript){: .float-right .v-align-text-top}
