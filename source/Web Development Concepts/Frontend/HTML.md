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

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

{: .note }
> By [Victor Hsiao](https://www.linkedin.com/in/hsiaovictor/)

HTML serves as the building blocks for our website. It represents the different pieces for your LEGO figure, the head, arms, body, legs.

Every HTML page ends with ".html", where each page has the same starting structure

```
<!doctype html>
<html lang="en-US">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width" />

    <title>My page title</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body></body>
</html>
```

Most HTML tags are structured like this:

![](https://clearlydecoded.com/assets/images/posts/2017-09-04-anatomy-of-html-tag/html-tag-attributes.png)

### The <head> tag

The head tag represents the set up for our HTML page

The two main components included in every `<head>` tag are the `<title>` and `<link>` tags

We use the `<title>` tag when we include a title for our webpage

We use the `<link>` tag for when we want to link a CSS stylesheet to our page, from the example above, we link the "style.css" stylesheet to our HTML page

We will outline the multiple components that every HTML website has:

### The header tags

Header tags represent the titles of our HTML

There are 6 different types of header tags: h1, h2, h3, h4, h5, and h6

To use a header tag, you would do:

```<h + "number">(content here)</h + "number">``` (where number is from 1 to 6)

![](https://th.bing.com/th/id/R.f31151c9930cad0b53977ddf32d16c4d?rik=RvEoDf4v8g7cUA&riu=http%3a%2f%2fictacademy.com.ng%2fwp-content%2fuploads%2f2017%2f10%2fHeading-Tag-Hierarchy.jpg&ehk=38aWjqrzDxhB1GMnv1P4RIyBArTDY3czYf0xm8uapJw%3d&risl=&pid=ImgRaw&r=0)

### The `<p>` tag

The `<p>` tag is used for big blocks of text, or paragraphs. We use it when we want to include big blocks of text on our website, like for a blog or article

```<p>(insert some text here)</p>```

![p tag](https://blog.hubspot.com/hs-fs/hubfs/Google%20Drive%20Integration/Using%20the%20%3Cp%3E%20Tag%20in%20HTML-1.png?width=657&name=Using%20the%20%3Cp%3E%20Tag%20in%20HTML-1.png)

### The `<a>` tag

The `<a>` tag is a tag is used to link other webpages or websites. 

To use an `<a>` tag, you have to specify the href attribute, which is the url that the tag links to.

```<a href="some url">(content here)</a>```

In between the opening and closing `<a>` tags, you insert some text that serves as the link. The default blue color text with the underline shows that the text is a link.

### The list tags

There are two types of lists in HTML:

1. ordered lists
2. unordered lists

#### **Ordered Lists**

To specify an unordered lists, you use the `<ol>` tag.

With ordered lists, your list items would be in a certain order, going from 1, 2, 3, 4, and so forth

![ordered list](https://th.bing.com/th/id/OIP.Cpx_G8zpj83y636HSsMcrgHaFj?rs=1&pid=ImgDetMain)

Same as ordered lists, to add items to your unordered list you use the `<li>` tag.

#### **Unordered Lists**

To specify an unordered lists, you use the `<ul>` tag.

Same as ordered lists, to add items to your unordered list you use the `<li>` tag.

Instead of ordered numbers, there would be a bullet point or some form of separator at the front of each list item

Unordered lists would look like this:

![unordered list](https://th.bing.com/th/id/OIP.HfkBXgQPgATQswMMF43-bwHaEJ?rs=1&pid=ImgDetMain)

### The `<img>` tag

The `<img>` tag is used to add images to our website.

Unlike the other tags, the image tag does not have a self-closing tag, so instead of ending with ```</img>``` we just end with ```/>```

```<img src="image link" alt="describe image here" />```

![](https://www.codewithfaraz.com/img/image%20tag%20in%20html%20how%20to%20add%20images%20in%20html%20-%20a%20beginners%20guide.jpg)

**To learn more about HTML, down below are some resources:**

[HTML on W3Schools](https://www.w3schools.com/html)
[Mozilla HTML Documentation](https://developer.mozilla.org/en-US/docs/Web/HTML)


[Previous: Frontend](../Frontend){: .float-left .v-align-text-top}
[Next: CSS](CSS){: .float-right .v-align-text-top}
