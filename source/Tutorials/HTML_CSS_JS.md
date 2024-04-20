---
layout: default
title: HTML, CSS, and Javascript
nav_order: 2
permalink: Tutorials/HTML_CSS_JS
parent: Tutorials
has_toc: true
---

{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

{: .note }

## Introduction

Welcome to the world of Web development! Whats the website you visit the most? What browser do you use to surf with? Have you ever wondered all these websites are made, or wanted to create your own? Despite all the different content and design you see in the web, webpages are primarily be broken down to three major components, namingly HTML ("Hypertext Markup Language"), CSS ("Cascading Style Sheets") and JS ("JavaScript"). Ultimately, these are all texts that are translated to tell the computer how to structure (HTML), style (CSS), and define and implement functionality (JS). We use these three separate technologies to add each component to the website and work very closely. Whether you are builing a simple personal webpage about yourself, or a complicated web application, you will need the same three core languages.

### HTML
If we imagine the web as a house, HTML lays the foundation and blueprint of the house. Essentially its just text It consists of "tags" enclosed in angle brackets, like ``<tag>``. Tags define structure and content. There are so many different types of tags, from defining lines and headings, links, forms, images and videos down to a simple text as the ones you are reading right now. These tags create a layout of the webpage.

- **Basic Structure**: An HTML document consists of elements enclosed in tags. Key elements include `<html>`, `<head>`, and `<body>`.
- **Content Elements**: HTML offers various elements for content like headings (`<h1>` to `<h6>`), paragraphs (`<p>`), lists (`<ul>`, `<ol>`, `<li>`), links (`<a>`), images (`<img>`), and more.
- **Semantic HTML**: Semantic HTML elements convey meaning, aiding accessibility and SEO.

### CSS
Every house has an architecture style, or a color scheme. All the rooms would follow that scheme according to the what the house should look like. Wouldn't it be nice to define that in once place? If we have the scheme defined in some place, all the pages we create with HTML would have that style without  specifying them repeteadly. This is where CSS comes in. It adds colors, fonts, spacing and styles of the elements used in HTML.

- **Selectors**: CSS selectors target HTML elements for styling. They can be simple (like element selectors), class-based (using `.class`), or ID-based (using `#id`).
- **Box Model**: CSS box model comprises content, padding, border, and margin, influencing element layout.
- **Styling Properties**: CSS properties like `color`, `font-size`, `background`, `margin`, and `padding` offer control over appearance.
- **Selectors Specificity**: Specificity determines which styles apply when multiple rules target the same element.

### JavaScript
Now that we've created a structure and style, we would want functionality and interaction. If we turn on the switch, what parts of the rooms will light up? Do you want your house to have automatic temperature adjusting to which part of the room you are in? JavaScript is the "code" of the webpage that defines and adds that functionality and behavior. It responds to the inputs and actions user gives, and creates outputs.

- **Basic Syntax**: JavaScript syntax includes variables, data types, operators, functions, and control structures like `if` statements and loops.
- **DOM Manipulation**: JavaScript interacts with the DOM (Document Object Model), enabling dynamic content updates and element manipulation.
- **Event Handling**: JavaScript responds to user interactions like clicks and keystrokes, triggering actions or behavior changes.
- **Asynchronous Operations**: JavaScript handles asynchronous tasks like fetching data from servers or APIs using promises or async/await.








> By [Victor Hsiao](https://www.linkedin.com/in/hsiaovictor/) 

When we want to add CSS styling to any of our HTML elements, to select the specific HTML elements we want to style, we would use one of the two types of CSS selectors

#### **ID Selectors**

You would use id selectors if you only want to apply CSS styling to one HTML element

To use an id selector, in your HTML, you use the id attribute

`<h1 id="any_id">Hello World!</h1>`

And in your CSS, you would use the `#` tag to select the element with a certain id

```
#any_id {
    (insert styles here)
}
```

Only one element can have a certain id, you cannot have two elements with the same id

#### **Class Selectors**

Class selectors allow you to apply the same style attributes to multiple elements

In your HTML, you would assign the class attribute to the tags you want to have the same style

From the below example, we see that two `<p>` tags can have the same class, in this case, "paragraph"

```
<h1>Hello, my name is Deadpool!</h1>
<p class="paragraph">I am an antihero, I have done good but have also done bad</p>
<p class="paragraph">I am played by Ryan Reynolds!</p>
```

To add style attributes to a class, we use the `.` tag instead

```
.paragraph {
    (insert styles here)
}
```

_______________________________________________________________

[Previous: Getting Started](Getting Started){: .float-left .v-align-text-top}
[Next: Python](Python){: .float-right .v-align-text-top}

