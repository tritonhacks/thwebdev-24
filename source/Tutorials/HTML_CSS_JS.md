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

