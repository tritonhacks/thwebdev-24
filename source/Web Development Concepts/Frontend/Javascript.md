---
layout: default
title: Javascript
nav_order: 3
permalink: Web Development Concepts/Frontend/Javascript
grand_parent: Web Development Concepts
parent: Frontend
has_children: false
---

# What is Javascript (JS)?
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

JavaScript is a programming language that works hand in hand with HTML and CSS, forming the backbone of most websites you visit. Think of HTML as the basic structure of your LEGO set, CSS as the colors and styles you apply to your LEGO pieces, and JavaScript as the motor that powers your moving LEGO constructions.

## Unleashing the Power of JavaScript

To add JavaScript to your website, you would want to use the `<script>` tag

You could place the `<script>` tag either in the `<head>` tag or in the `<body>` tag, but in this case we would add it to the `<body>` tag to have our JavaScript interact with our HTML and CSS.

To add **internal** JavaScript to your website, you would insert the JS code directly, as shown below:

```
<!DOCTYPE html>
<html lang="en-US">
 
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Today's Date</title>
</head>
 
<body>
  <script>
      let d = new Date();
      document.body.innerHTML = "<h1>Today's date is " + d + "</h1>"
  </script>
</body>
 
</html>
```

However, like with our CSS, we would want to keep our JavaScript separate from our HTML, so best practice is to use **external** JavaScript, or store it in a separate file.

To add **external** JavaScript to your website, or have it in a separate file you would have:

```<script src="myscript.js"></script>```

You would create a JavaScript file using the extension `.js`, and would ideally want to store it in a separate folder from the HTML. The `<script>` tag would be the last tag in the `<body>` section, as shown in the example block of code down below

```
<!DOCTYPE html>
<html lang="en-US">
 
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Today's Date</title>
</head>
 
<body>
   <script src="path/to/my/script.js"></script>
</body>
 
</html>
```

This will connect our JavaScript to our HTML and CSS, giving us the power to create a fully dynamic website!

## The Building Blocks of JavaScript

JavaScript offers a toolkit of functions and features to bring websites to life. Let's dive into the exciting world of JavaScript and discover its fundamental components!

### Query Selectors

Query selectors allow you to collect information and manipulate certain HTML tags

There are four main query selectors: `getElementById`, `getElementsByClassName`, `getElementsByTagName`, and `querySelector`

You would use the `querySelector` function whenever you want to get the first match of a certain element

This selector below is if you want your JavaScript to work with an `<h1>` tag 

**Ex:** ```document.querySelector("h1");```

For the `getElementById` tag, you would use it to get an element with a certain id attribute. 

Remember, only one element can have an id attribute

**Ex:**
```
<!DOCTYPE html>
<html lang="en-US">
 
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Today's Date</title>
</head>
 
<body>
    <h1 id="title">Today's Date</h1>
    <script>
        let header = document.getElementById("title");
    </script>
</body>
 
</html>
```

For the `getElementsByClassName` function, you would use it to get elements with a certain class name.

Remember, multiple elements can have the same class name. This function will return an array of the elements with a certain class name.

**Ex:** ```let ex = document.getElementsByClassName("example");```

The `getElementsByTagName` function works similar to the `getElementsByClassName` function, except you use it to get certain **elements**

**Ex:** ```let list_items = document.getElementsByTagName("li");```

### Variables

Variables are containers that can store different values. The values it can store ranges from numbers, strings, etc.

You would declare a variable using the `let` keyword, and assign it a value using the `=` sign

Down below are some examples of variables

```
let name = "Victor";
let age = 19;
let isStudent = true;
```

You can reassign the variable later in the code

```
let name = "Victor";
name = "Steve";
```

### Functions

Functions are containers that store **a block of code**. They are helpful when you want to run a certain block of code multiple times.

To define a function, you would use the `function` keyword, the name of the function after it and then parentheses `()`. Inside the parentheses would be different parameters, or values you want to pass into the function.

`Ex (function signature): function printName(name)`

The function code would be contained within curly brackets `{ }`, so our overall function would look something like this:

```
function printName(name) {
    console.log("Hello " + name);
}
```

### Conditionals

Conditionals are represented by an `if` statement. You use them if you want to check or compare something.

**Ex:**

```
let name = "Bob";

if (name == "Bob") {
    console.log("Hi Bob!");
}
```

We can also use the `else if` and `else` statements if we want to run code for if the initial if statement is not satisfied. We can only use `else if` and `else` if we already have an initial if statement

**Ex:**

```
let name = "Bob";

if (name == "Bob") {
    console.log("Hi Bob!");
} else if (name == "Victor") {
    console.log("Hi Victor!");
} else {
    console.log("Who are you?");
}
```

### Loops

There are two different types of loops: while loops and for loops

While loops are when you want to run code while a certain condition is met

**Ex:**

```
let seconds = 5;

while (seconds >= 0) {
    console.log(seconds);
    seconds -= 1;
}
```

For loops are when you want to iterate through something, like the characters of a string or a list of values, or when you want to run a certain line of code a set number of times.


**Ex:**

```
let fruits = ['apple', 'banana', 'orange', 'grape'];

for (int i = 0; i < fruits.length; i++) {
    console.log(fruits[i]);
}
```

### Comments

You can have single or multi-line comments

```
// This is a single line comment

/*

This is a multi line comment
This is a multi line comment

*/
```

[Previous: CSS](CSS){: .float-left .v-align-text-top}
[Next: Backend](../Backend){: .float-right .v-align-text-top}
