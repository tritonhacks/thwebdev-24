---
layout: default
title: HTML, CSS, and Javascript
nav_order: 2
permalink: Tutorials/HTML_CSS_JS
parent: Tutorials
has_toc: false
---

{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

{: .note }

> By [Victor Hsiao](https://www.linkedin.com/in/hsiaovictor/) 

## HTML

### **The `<head>` tag**

The head tag represents the set up for our HTML page

The two main components included in every `<head>` tag are the `<title>` and `<link>` tags

We use the `<title>` tag when we include a title for our webpage

We use the `<link>` tag for when we want to link a CSS stylesheet to our page, from the example above, we link the "style.css" stylesheet to our HTML page

We will outline the multiple components that every HTML website has:

### **The header tags**

Header tags represent the titles of our HTML

There are 6 different types of header tags: h1, h2, h3, h4, h5, and h6

To use a header tag, you would do:

```<h + "number">(content here)</h + "number">``` (where number is from 1 to 6)

![](https://th.bing.com/th/id/R.f31151c9930cad0b53977ddf32d16c4d?rik=RvEoDf4v8g7cUA&riu=http%3a%2f%2fictacademy.com.ng%2fwp-content%2fuploads%2f2017%2f10%2fHeading-Tag-Hierarchy.jpg&ehk=38aWjqrzDxhB1GMnv1P4RIyBArTDY3czYf0xm8uapJw%3d&risl=&pid=ImgRaw&r=0)

### **The `<p>` tag**

The `<p>` tag is used for big blocks of text, or paragraphs. We use it when we want to include big blocks of text on our website, like for a blog or article

```<p>(insert some text here)</p>```

![p tag](https://blog.hubspot.com/hs-fs/hubfs/Google%20Drive%20Integration/Using%20the%20%3Cp%3E%20Tag%20in%20HTML-1.png?width=657&name=Using%20the%20%3Cp%3E%20Tag%20in%20HTML-1.png)

### **The `<a>` tag**

The `<a>` tag is a tag is used to link other webpages or websites. 

To use an `<a>` tag, you have to specify the href attribute, which is the url that the tag links to.

```<a href="some url">(content here)</a>```

In between the opening and closing `<a>` tags, you insert some text that serves as the link. The default blue color text with the underline shows that the text is a link.

### **The list tags**

There are two types of lists in HTML:

1. ordered lists
2. unordered lists

### **Ordered Lists**

To specify an unordered lists, you use the `<ol>` tag.

With ordered lists, your list items would be in a certain order, going from 1, 2, 3, 4, and so forth

![ordered list](https://th.bing.com/th/id/OIP.Cpx_G8zpj83y636HSsMcrgHaFj?rs=1&pid=ImgDetMain)

Same as ordered lists, to add items to your unordered list you use the `<li>` tag.

### **Unordered Lists**

To specify an unordered lists, you use the `<ul>` tag.

Same as ordered lists, to add items to your unordered list you use the `<li>` tag.

Instead of ordered numbers, there would be a bullet point or some form of separator at the front of each list item

Unordered lists would look like this:

![unordered list](https://th.bing.com/th/id/OIP.HfkBXgQPgATQswMMF43-bwHaEJ?rs=1&pid=ImgDetMain)

### **The `<img>` tag**

The `<img>` tag is used to add images to our website.

Unlike the other tags, the image tag does not have a self-closing tag, so instead of ending with ```</img>``` we just end with ```/>```

```<img src="image link" alt="describe image here" />```

![](https://www.codewithfaraz.com/img/image%20tag%20in%20html%20how%20to%20add%20images%20in%20html%20-%20a%20beginners%20guide.jpg)

## CSS

When we want to add CSS styling to any of our HTML elements, to select the specific HTML elements we want to style, there are a few different type of CSS selectors we can use

### **Element Selectors**

### **ID Selectors**

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

### **Class Selectors**

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

### **Basic Style Attributes**

There are many different types of style attributes, but we'll lay out some basic ones.

When writing any CSS code, you have to write it like this:

![CSS basic style example](https://res.cloudinary.com/practicaldev/image/fetch/s--Uvc4p-Vs--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/edojfcbz6sr7j0b2l6v1.jpg)

The ones below are style attributes you would use for **text**

**font-size**: changes the size of the text (font size is based on pixels, or px)

`font-size: 16px;`

**color**: changes the color of the text

`color: blue;`

**font-family**: give a specific font to selected text, there are many different font styles out there (the default is sans-serif)

`font-family: sans-serif;`

**text-align**: controls how text is aligned on a page, can be aligned left, right, or center

`text-align: center;`

For a full list of CSS properties, visit the link below:

[All CSS properties](https://www.dofactory.com/css/properties)

## JavaScript

_______________________________________________________________

[Previous: Getting Started](Getting Started){: .float-left .v-align-text-top}
[Next: Python](Python){: .float-right .v-align-text-top}

