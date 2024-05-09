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

JavaScript is a programming language that works hand in hand with HTML and CSS, forming the backbone of most websites you visit. Think of HTML as the basic structure of your LEGO set, CSS as the colors and styles you apply to your LEGO pieces, and JavaScript as the motor that powers your moving LEGO constructions.

## Unleashing the Power of JavaScript
{: .no_toc} 

To add JavaScript to your website, you would want to use the `<script>` tag

You could place the `<script>` tag either in the `<head>` tag or in the `<body>` tag. We add it to the body tag for this example.

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


[Previous: CSS](CSS){: .float-left .v-align-text-top}
[Next: Backend](../Backend){: .float-right .v-align-text-top}
