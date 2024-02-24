---
layout: default
title: Cascading Style Sheets
has_children: false
parent: Frontend
permalink: /Frontend/CSS
nav_order: 2
---

# What are Cascading Style Sheets (CSS)?
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

{: .note }
> By [Victor Hsiao](https://www.linkedin.com/in/hsiaovictor/)    

We will now discuss different aspects of CSS

### Types of Styling

#### **Inline Styling**

Inline styling is when you add CSS styles inside an HTML tag

To do inline styling, you add the  `style` attribute inside an HTML tag, and then the specific CSS property inside the quotes of the style attribute, only do styling within the `<body>` tag, and inside the opening tag only (not in the closing tag)

`<h1 style="color:red">Hello!</h1>`

This is considered the most inefficient form of implementing CSS styles because if we want to implement multiple CSS properties, it can get pretty jumbled and messy!

#### **Internal Styling**

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

#### **External Styling**

For external CSS styling, we use the ```<link>``` tag, which we add to the ```<head>``` section in our HTML

```<link rel="stylesheet" href="(name of css file).css" />```

We add the rel attribute and specify it as a "stylesheet" to specify that we want to add CSS code to our HTML, and then the href attribute to link our CSS code to the HTML

### Selecting Elements to Add CSS Styling To

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

Overall, CSS can make our website look pretty and stylish. Like with our LEGO figure, we can use CSS to make our website stand out in its own unique way!

[Previous: HTML](HTML){: .float-left .v-align-text-top}
[Next: Javascript](Javascript){: .float-right .v-align-text-top}
