---
layout: default
title: Hypertext Markup Language
has_children: false
parent: Frontend
permalink: /Frontend/HTML
nav_order: 1
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

### The <head> tag

The head tag represents the 

We will outline the multiple components that every HTML website has:

### Header Tags

Header tags represent the titles of our HTML

There are 6 different types of header tags: h1, h2, h3, h4, h5, and h6

To use a HTML tag, you would do:

```<h + "number">(content here)</h + "number">``` (where number is from 1 to 6)

![](https://th.bing.com/th/id/R.f31151c9930cad0b53977ddf32d16c4d?rik=RvEoDf4v8g7cUA&riu=http%3a%2f%2fictacademy.com.ng%2fwp-content%2fuploads%2f2017%2f10%2fHeading-Tag-Hierarchy.jpg&ehk=38aWjqrzDxhB1GMnv1P4RIyBArTDY3czYf0xm8uapJw%3d&risl=&pid=ImgRaw&r=0)

### Paragraph Tags

The paragraph tag is used for big blocks of text

### Link Tags

The link tag is used to provide a link to other webpages or websites

### Image Tags

Unlike the other tags, the image tag does not have a self-closing tag, so instead of ending with ```</img>``` we just end with ```/>```

```<img src="image link" alt="describe image here" />```

[Previous: Frontend](../Frontend){: .float-left .v-align-text-top}
[Next: CSS](CSS){: .float-right .v-align-text-top}
